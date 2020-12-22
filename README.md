# Learning-Webpack-Advanced (Recap)

## Core concepts
1. entry
  - single entry (shorthand)
  - object syntax
  - separate app and vendor entries
2. output
  - for multiple entry points
    - `output: { filename: '[name].[contenthash].bundle.js' }`
    - `[contenthash] is used for cache bustling.
3. loader
  - webpack only understands JavaScript and JSON files.
  - loaders allow webpack to process other types of files and convert them into valid modules that can be consume by your application and added to the dependency graph.
  - Example loaders: 
    - 'style-loader'
    - 'css-loader'
    - 'MiniCssExtractPlugin.loader' -> Extract css file from bundle file
    - 'file-loader'
    - 'html-loader'
4. plugins
  - plugins can be leveraged to perform a wider range of tasks like bundle optimization, asset management and injection of environment variables.
  - Example plugins:
    - 'html-webpack-plugin' -> generate a HTML file including the bundle files using a script tag.
    - 'clean-webpack-plugin' -> remove all file inside webpack's output.path directory, as well as all unused webpack assets after every successful rebuild.
    - 'mini-css-extract-plugin'
