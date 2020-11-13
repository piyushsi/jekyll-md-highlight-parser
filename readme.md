# jekyll-md-highlight-parser

A [Jekyll](https://jekyllrb.com/) Markdown Highlight parser.

## Installation

```
$ npm install jekyll-md-highlight-parser
```

## Usage

```javascript
import { mdParse } from "jekyll-md-highlight-parser";
console.log({string,mdParse:mdParse(string)};

// using ReactMarkdown && CodeBlock

<ReactMarkdown
  escapeHtml={true}
  source={mdParse(string)}
  renderers={{ code: CodeBlock }}
></ReactMarkdown>;
```

## Badges

[![npm version][npm-badge-url]][npm-url]

[npm-badge-url]: https://img.shields.io/npm/v/jekyll-md-highlight-parser.svg
[npm-url]: https://www.npmjs.com/package/jekyll-md-highlight-parser

## License

[MIT](LICENSE)
