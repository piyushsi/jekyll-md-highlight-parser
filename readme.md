# jekyll-md-highlight-parser

A [Jekyll](https://jekyllrb.com/) Markdown Highlight && Image parser.

## Installation

```
$ npm install jekyll-md-highlight-parser
```

## Usage

```javascript
let mdJekyll = `{% highlight ruby %}
puts "I love ice cream"
{% endhighlight %}`;

// Parse Highlight using ReactMarkdown && CodeBlock
import { hParse } from "jekyll-md-highlight-parser";

<ReactMarkdown
  escapeHtml={true}
  source={mdParse(mdJekyll)}
  renderers={{ code: CodeBlock }}
></ReactMarkdown>;

// Parse Highlight with image using ReactMarkdown
import { hParse, iParse } from "jekyll-md-highlight-parser";
<ReactMarkdown
  escapeHtml={true}
  source={iParse(hParse(mdJekyll))}
  renderers={{ code: CodeBlock }}
></ReactMarkdown>;
```

## Badges

[![npm version][npm-badge-url]][npm-url]

[npm-badge-url]: https://img.shields.io/npm/v/jekyll-md-highlight-parser.svg
[npm-url]: https://www.npmjs.com/package/jekyll-md-highlight-parser

## License

[MIT](LICENSE)
