# fa-extract
A tool to extract only used icons from Font Awesome JS/SVG icons sets.

This should be considered a quick and dirty hack, a *pre-alpha* code. I use it to make my Font Awesome JS file smaller but YMMV.

## Install
```
composer create-project spaze/fa-extract path/to/install
```

E.g.
```
composer create-project spaze/fa-extract vendor/spaze/fa-extract
```

Or wherever. This is installed as a *project*, not a library, because it's not a library.
Your project code is not calling it directly and it might have a dependencies in the future that might collide with your project dependencies.

## Usage
```
php vendor/spaze/fa-extract/bin/fa-extract . ~/desktop/fontawesome-free-5.9.0-web > used.js
```

## Minify
You can minify the output (`used.js` above) using [Closure Compiler](https://closure-compiler.appspot.com/home) to save roughly 50% of the file size.
