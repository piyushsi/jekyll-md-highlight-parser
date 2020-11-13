# jekyll-md-highlight-parser

A [Jekyll](https://jekyllrb.com/) Markdown Highlight parser.

## Installation

```
$ npm install jekyll-md-highlight-parser
```

## Usage

```javascript
let mdJekyll = `{% highlight ruby %}
puts "I love ice cream"
{% endhighlight %}`;
import { mdParse } from "jekyll-md-highlight-parser";
console.log({ mdJekyll, mdParse: mdParse(mdJekyll) });

// using ReactMarkdown && CodeBlock

<ReactMarkdown
  escapeHtml={true}
  source={mdParse(mdJekyll)}
  renderers={{ code: CodeBlock }}
></ReactMarkdown>;
```

## Badges

[![npm version][npm-badge-url]][npm-url]

[npm-badge-url]: https://img.shields.io/npm/v/jekyll-md-highlight-parser.svg
[npm-url]: https://www.npmjs.com/package/jekyll-md-highlight-parser

## License

[MIT](LICENSE)
