# raml2html-docson

This project is the playground for building [raml2html](https://github.com/raml2html/raml2html)
templates using [docson](https://github.com/lbovet/docson) for rendering [json-schemas](http://json-schema.org).

## Before you begin

```
npm install -g raml2html
npm install -g http-server
```

## Build documentation

*Note*: the output html file **must** be generated in the root folder of the
project because of the relative links.

```
raml2html --template raml2html_templates/template.nunjucks --input examples/github.raml --output github.html
http-server
open http://127.0.0.1:8080/github.html
```

## Known bugs

* As `requirejs` load file asynchronously and `jquery` need to be loaded **before**
`bootstrap`, an error can occur. To fix it must be find the way to load js files
in order. The workaround is not to enable browser caching and press F5

## Notes

```
wget https://github.com/lbovet/docson/tarball/4c5e24a72e94e7cb2d5cc0d4391556690dc4d5d6 -O 4c5e24a72e94e7cb2d5cc0d4391556690dc4d5d6.tgz
tar zxf 4c5e24a72e94e7cb2d5cc0d4391556690dc4d5d6.tgz
mv lbovet-docson-4c5e24a/ docson
cd contrib
wget https://netdna.bootstrapcdn.com/bootstrap/3.1.1/js/bootstrap.min.js
wget https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.3.0/highlight.min.js
```
