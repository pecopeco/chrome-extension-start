# chrome-extension-start

> Chrome 拓展模板

## Build Setup

``` bash
# install dependencies
npm i

# serve with auto reload && import the **dist** folder in the Chrome browser
npm start

# build for production with minification && crx package
npm run build
```

由于 wcer 组件在 nodejs v8.15.0 版本以上无法正常运行，调试期间需注释掉 webpack.base.conf.js 中的：

```
new ChromeReloadPlugin({
  port: 23333,
  manifest: resolve('src/manifest.js')
})
```

build 时需重新开启
