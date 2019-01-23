marked-iterm
===

> marked-terminal不支持将图片显示在控制台中，marked-iterm在marked-terminal的基础上添加了显示图片的功能(仅支持本地图片)

## Install

```sh
npm install marked marked-iterm
```

## Example

```javascript
var marked = require('marked');
var TerminalRenderer = require('marked-iterm');

marked.setOptions({
  renderer: new TerminalRenderer()
});

console.log(marked("![图片](./images/logo.png '500px*500px')"));
```
