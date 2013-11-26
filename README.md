urturn-expression-css
=====================

Base CSS for Urturn expressions

- [style.css](http://urturn.github.io/urturn-expression-css/css/style.css): normalize.css + urturn classes + buttons + icons
- [style_edit.css](http://urturn.github.io/urturn-expression-css/css/style_edit.css): normalize.css + urturn classes + forms + urturn edit classes + buttons + icons
- [style_play.css](http://urturn.github.io/urturn-expression-css/css/style_play.css): normalize.css + urturn classes + buttons
- [icons.css](http://urturn.github.io/urturn-expression-css/css/icons.css)

Build & Deploy
--------------
`rake install` will install a git pre-commit hook that will ensure css is generated.
`rake compile` will compile the sass source.
`rake publish` will take the commited code and create a new tag in the repository.

Update the fonts files
----------------------
* Replace the files in fonts folder with the new ones
* Copy the .icon_***:before classes (like .icon_activity:before) from the the style.css newly generated into icons.scss by replacing the actuals
* Change the version in bower.json
* refer to build and deploy for compiling and publishing

Credits
-------

- [LeBenLeBen](http://github.com/LeBenLeBen)
- [Template](http://github.com/stephband/template) by [stephband](http://github.com/stephband)
- [Normalize.css](http://necolas.github.com/normalize.css/) by [Nicolas Gallagher](http://nicolasgallagher.com/), co-created with [Jonathan Neal](http://music.thewikies.com/jonneal/)
