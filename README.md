Lity
====

Lity is a ultra-lightweight and responsive lightbox plugin which supports
images, iframes and inline content out of the box.

Minified and gzipped, its total footprint weights about 2kB.

It works with [jQuery](http://jquery.com) and [Zepto](http://zeptojs.com).

If you need to be compatible with IE8, use the
[es5-shim](https://github.com/es-shims/es5-shim).

Installation
------------

Include the Lity javascript and css files and its dependencies in your HTML
document (if your using Lity with image links,
[imagesLoaded](http://imagesloaded.desandro.com) is required):

```html
<link href="dist/lity.css" rel="stylesheet">
<!-- Remove the following line if you do not need IE8 support -->
<!--[if lt IE 9]><script src="lib/es5-shim.js"></script><![endif]-->
<script src="lib/jquery.js"></script>
<script src="lib/imagesloaded.pkgd.js"></script>
<script src="dist/lity.js"></script>
```

Usage
-----

Add the `data-lity` attribute to `<a>` elements for which you want the links to
be opened in a lightbox:

```html
<a href="https://farm9.staticflickr.com/8642/16455005578_0fdfc6c3da_b.jpg" data-lity>Image</a>
<a href="#inline" data-lity>Inline</a>
<a href="//www.youtube.com/watch?v=XSGBVzeBUbk" data-lity>iFrame Youtube</a>
<a href="//vimeo.com/1084537" data-lity>iFrame Vimeo</a>
<a href="//maps.google.com/maps?q=1600+Amphitheatre+Parkway,+Mountain+View,+CA" data-lity>Google Maps</a>

<div id="inline" style="background:#fff" class="lity-hide">
    Inline content
</div>
```

License
-------

Copyright (c) 2015 Jan Sorgalla.
Released under the [MIT](LICENSE?raw=1) license.
