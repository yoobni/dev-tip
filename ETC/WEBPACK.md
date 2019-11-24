# Webpack 2

* 웹팩 2.0
* webpack.config
* reslove.alias 부분과  module.rules의 expose-loader 의 설정을 추가.

#### webpack.config.js

```
const webpack = require('webpack');
const {resolve, join} = require('path');
const CleanWebpackPlugin = require('clean-webpack-plugin');
const UglifyJSPlugin = require('uglifyjs-webpack-plugin');
const HtmlWebpackPlugin = require('html-webpack-plugin');
const ExtractTextPlugin = require('extract-text-webpack-plugin');
const ExtractCSS = new ExtractTextPlugin('css/style.css');

module.exports = {
    entry: {
        jquery: 'jquery',
        appMain: './src/entry.js'
    },
    output: {
        path: resolve(__dirname, 'dist'),
        filename: 'modules/[name].js'
    },
    plugins: [
        new CleanWebpackPlugin(['dist']),
        new UglifyJSPlugin({compress: true, exclude: 'jquery'}),
        new HtmlWebpackPlugin({
            template: './src/index.html',
            chunks: ['appMain', 'jquery'],
            chunksSortMode: function (a, b) {
                if (a.names[0] > b.names[0]) {
                    return -1;
                }
                if (a.names[0] < b.names[0]) {
                    return 1;
                }
                return 0;
            },
            minify: {
                collapseWhitespace: true,
                removeComments: true,
                keepClosingSlash: true,
                xhtml: true
            }

        }),
        ExtractCSS
    ],
    resolve: {
        alias: {
            bxslider: resolve(__dirname, 'node_modules/bxslider/dist/jquery.bxslider.js')
        }
    },
    module: {
        rules: [
            { test: /\.js$/, use: [
                {loader: 'babel-loader', options: {
                    presets: [
                        ['env', {targets: {browsers:['ie 9']}}]
                    ]
                }},
                {loader: 'webpack-strip', options: {strip: ['console.log']}}
            ], exclude: /node_modules/},

            {test: /\.css$/, use: ExtractCSS.extract({
                    fallback: 'style-loader',
                    use: [
                        {loader: 'css-loader', options: {minimize: true}},
                        {loader: 'postcss-loader', options: { plugins: function () { return [ require('autoprefixer')]}}}
                    ]
                })
            },
            { test: /\.(jpe?g|gif|png)$/, use: [
                {loader: 'file-loader', options: {name:'images/[folder]/[name].[ext]'}},
                {loader: 'image-webpack-loader', options: {
                        progressive: true, optimizationLevel: 7, interlaced: true,
                        pngquant: {quality: '65-80', speed: 4}
                }}
            ]},
            { test: /\.html$/, use: [
                {loader: 'html-loader', options: {attrs: ['img:src']}}
            ]},
            { test: require.resolve('jquery'), loader: 'expose-loader?$!expose-loader?jQuery!expose-loader?window.$!expose-loader?window.jQuery'},
        ]
    }
};
```


#### entry.js
```
import './css/basic.css';
import './css/layout.css';

import 'bxslider';
import './modules/sly';

$(document).ready(function () {
    console.log($('#root').bxSlider());
        //output - [div#root, context: document, selector: "#root"]  --> bxslider 메서드가 추가되었다.

    var $frame  = $('#frame');
    var $slidee = $frame.children('ul').eq(0);
    var $wrap   = $frame.parent();

    $frame.sly({
        horizontal: 0,
        itemNav: 'basic',
        smart: 1
    });
});
```
