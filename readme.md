#Better CSS syntax highlight for Sublime Text 2

CSS syntax highlight in Sublime Text 2 is far from complete. This project's goal is to fix this.

The highlight is based on [validation rules](http://jigsaw.w3.org/css-validator/). However, not all properly highlighted code will be valid. If you want to better check your CSS, you probably should use [CSS Lint plugin](//github.com/austinhappel/sublime-csslint).

##Changes

###Updated

* type selectors
* property names (incl. aural)
* property value keywords (incl. aural)

###Fixed

* pseudo-element selector (no more than two semicolons will be highlighted)
* missing `:only-child`

###Removed

* font-family names, except generic ones

##Installation

1. Open `Preferences` → `Browse Packages...` → `CSS`
2. Backup original `CSS.tmLanguage` and replace it with `CSS.tmLanguage` from this repository

##Roadmap

* complete function highlight (gradients, transforms, etc)
* highlight keyword that can't come alone (i. e. `inset`, `hanging`)