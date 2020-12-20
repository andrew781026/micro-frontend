# vue-cli-front

研究 vue-cli 產出的 js 與 css 可以如何的做成 custom tag

利用 `vue.config.js` 可以設定 .js.map 不產出 , 減少檔案數量

```javascript
// vue.config.js
module.exports = {
  productionSourceMap: false
};
```

dist 中產生的 chunk-venders.xxx.js 代表由 node_modules 來的套件 , 都放在這個 js 中 ( ex : vue.js )

之後還要思考要如何與 JSP . ASP 的驗證系統作融合 ? 

## Micro Frontends 相關討論文章

- [一起探討 Micro Frontends 的世界](https://blog.techbridge.cc/2019/01/12/micro-frontends-concept/)
- [11 Micro Frontends Frameworks You Should Know](https://itnext.io/11-micro-frontends-frameworks-you-should-know-b66913b9cd20)
- [Will 保哥討論微前端 with Angular](https://hackmd.io/@ModernWeb/2020/%2F%40ModernWeb%2FSkGoGWqUD)
- [Vue Web Component](https://cli.vuejs.org/guide/build-targets.html#web-component)