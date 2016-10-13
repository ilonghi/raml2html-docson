# raml2html-docson

```
wget https://github.com/lbovet/docson/tarball/4c5e24a72e94e7cb2d5cc0d4391556690dc4d5d6 -O 4c5e24a72e94e7cb2d5cc0d4391556690dc4d5d6.tgz
tar zxf 4c5e24a72e94e7cb2d5cc0d4391556690dc4d5d6.tgz
mv lbovet-docson-4c5e24a/ docson
cd contrib
wget https://netdna.bootstrapcdn.com/bootstrap/3.1.1/js/bootstrap.min.js
wget https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.3.0/highlight.min.js
```
```
raml2html --template raml2html_templates/template.nunjucks --input examples/github.raml --output github.html
```
