# jk-markdown-it  

<p>
  <img alt="JK" src="https://img.shields.io/badge/-JK-brightgreen">
  <a href="https://github.com/traceslord/jk-markdown-it">
    <img alt="code size" src="https://img.shields.io/github/languages/code-size/traceslord/jk-markdown-it">
  </a>
  <img alt="version" src="https://img.shields.io/github/package-json/v/traceslord/jk-markdown-it">
  <a href="https://github.com/traceslord/jk-markdown-it/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/traceslord/jk-markdown-it" alt="license">
  </a>
</p>

> A Javascript Markdown to HTML converter.

## Installation
```
npm install jk-markdown-it --save
```

## Usage examples
引入 `index.js` ：
```html
<div class="jk-markdown-it"></div>
```

```js
import markdownIt from "jk-markdown-it";
import "jk-markdown-it/styles/markdown-it.css";
const html = markdownIt("## md");
const jkMarkdownIt = document.getElementsByClassName("jk-markdown-it")[0];
jkMarkdownIt.innerHTML = html;
```

引入 `vue` 组件：
```html
<markdown-it :md="value"></markdown-it>
```

```js
import MarkdownIt from "jk-markdown-it/MarkdownIt.vue";

export default {
  components: {
    MarkdownIt
  },
  data() {
    return {
      value: "## md"
    };
  }
};
```

## Plugin list  
* highlight.js
* markdown-it
* markdown-it-abbr
* markdown-it-container
* markdown-it-deflist
* markdown-it-emoji
* markdown-it-footnote
* markdown-it-ins
* markdown-it-katex
* markdown-it-mark
* markdown-it-sub
* markdown-it-sup
* markdown-it-task-lists

## License
[MIT](https://github.com/traceslord/jk-markdown-it/blob/master/LICENSE)

Copyright (c) 2020-present zhuhuajian
