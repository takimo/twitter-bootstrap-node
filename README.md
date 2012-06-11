twitter-bootstrap-node
======================

Twitter Bootstrap for Node.js(now only support express template)

This tool can build template that support 'Twitter Bootstrap'

## Installation

    $ npm install -g twitter-bootstrap-node

## Quick Start

Create the project:
(Default css engine is "less",And template engine is "jade")

    $ twitter-bootstrap project
    $ cd project
    $ npm install
    $ node app.js

![command screen shot](http://cdn-ak.f.st-hatena.com/images/fotolife/t/takimo/20120609/20120609111814.png)

Change template engine:

    $ twitter-bootstrap -t ejs project

# Future
  * build template(not only supported express template)
  * bootstrap's image files copy to "public/images/bootstrap/"
  * CSS(bootstrap.css or bootstrap.min.css) is dynamically built using "Less" 

# What should add "bootstrap.css/bootstrap.min.css" where? 

bootstrap.css(bootstrap.min.css) is as 'public/stylesheets/style.css' that already added views/layout.jade(layout.ejs)

```css
// public/stylesheets/style.css
@import "bootstrap.less";
// Padding for fixed-navbar
body {
padding-top: 60px;
padding-bottom: 40px;
}
@import "responsive.less";
@iconSpritePath: "/images/bootstrap/glyphicons-halflings.png";
@iconWhiteSpritePath:     "/images/bootstrap/glyphicons-halflings-white.png";
```


## Based Application

  Express (bin/express)

  https://github.com/visionmedia/express

  Copyright (c) 2009-2011 TJ Holowaychuk &lt;tj@vision-media.ca&gt;

## License

(The MIT License)

Copyright (c) 2012 Shinya Takimoto &lt;shinya.takimoto@gmail.com&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
