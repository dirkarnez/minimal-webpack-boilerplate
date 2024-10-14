minimal-webpack-boilerplate
===========================
### CLI Documentation
- [webpack-cli/OPTIONS.md at master · webpack/webpack-cli](https://github.com/webpack/webpack-cli/blob/master/OPTIONS.md)

### Tutorials
- [How to Set Up webpack 5 From Scratch | Tania Rascia's Personal Website](https://www.taniarascia.com/how-to-use-webpack/)
- [taniarascia/webpack-boilerplate: 📦 ‎ A sensible webpack 5 boilerplate.](https://github.com/taniarascia/webpack-boilerplate)
- [Webpack 前端打包工具 - 使用 webpack-merge 區分 dev 與 prod 環境 | Roya's Blog](https://awdr74100.github.io/2020-04-09-webpack-webpackmerge/)
### TODOs
- [ ] Language-agnostic hot-reload
  - https://github.com/amilajack/erb-sqlite-example/blob/main/.erb/configs/webpack.config.renderer.dev.ts
  - [dirkarnez/minimal-iris-spa-hot-reload](https://github.com/dirkarnez/minimal-iris-spa-hot-reload)
- [ ] Webpack 5
  - https://github.com/Richienb/node-polyfill-webpack-plugin
  - [Webpack 5 : Guide for beginners - DEV Community](https://dev.to/anitaparmar26/webpack-5-guide-for-beginners-314c)
  - [Webpack 5 Node Polyfills Upgrade Cheatsheet](https://gist.github.com/ef4/d2cf5672a93cf241fd47c020b9b3066a)
  - [Resolve | webpack](https://webpack.js.org/configuration/resolve/#resolvefallback)
  - 
  - ```js
    module.exports = {
      //...
      resolve: {
        fallback: {
          assert: require.resolve('assert'),
          buffer: require.resolve('buffer'),
          console: require.resolve('console-browserify'),
          constants: require.resolve('constants-browserify'),
          crypto: require.resolve('crypto-browserify'),
          domain: require.resolve('domain-browser'),
          events: require.resolve('events'),
          http: require.resolve('stream-http'),
          https: require.resolve('https-browserify'),
          os: require.resolve('os-browserify/browser'),
          path: require.resolve('path-browserify'),
          punycode: require.resolve('punycode'),
          process: require.resolve('process/browser'),
          querystring: require.resolve('querystring-es3'),
          stream: require.resolve('stream-browserify'),
          string_decoder: require.resolve('string_decoder'),
          sys: require.resolve('util'),
          timers: require.resolve('timers-browserify'),
          tty: require.resolve('tty-browserify'),
          url: require.resolve('url'),
          util: require.resolve('util'),
          vm: require.resolve('vm-browserify'),
          zlib: require.resolve('browserify-zlib'),
        },
      },
    };
    ```
