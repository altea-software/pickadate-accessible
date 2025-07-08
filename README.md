# pickadate-accessible

*An accessible fork of the original [pickadate.js](https://github.com/amsul/pickadate.js) library*

The mobile-friendly, responsive, and lightweight jQuery date & time input picker with WCAG 2.1 AA compliance.

[![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/pickadate)


#### To get started, check out the:

[Homepage](http://amsul.ca/pickadate.js) - [Date picker](http://amsul.ca/pickadate.js/date) - [Time picker](http://amsul.ca/pickadate.js/time) - [API](http://amsul.ca/pickadate.js/api)


#### To get it:

[Download the latest stable build](https://github.com/altea-software/pickadate-accessible/archive/master.zip)

*or*

`git clone git://github.com/altea-software/pickadate-accessible.git`

*or*

`bower install pickadate`




<br>

## Library files

The `lib` folder includes the library files with a `compressed` folder containing the minified counter-parts. These files are minified using [Grunt](#building-with-grunt).

### Pickers

There are three picker files:

* `picker.js` The core file (required before any other picker)
* `picker.date.js` The date picker
* `picker.time.js` The time picker


### Themes

All themes are [generated using LESS](#less-styling) and compiled from the `lib/themes-source` folder into the `lib/themes` folder.

There are two themes:

* `default.css` The default modal-style theme
* `classic.css` The classic dropdown-style theme

Based on the theme, pick the relevant picker styles:

* `default.date.css` and `default.time.css` when using the default theme
* `classic.date.css` and `classic.time.css` when using the classic theme

__**__ For languages with text flowing from right-to-left, also include the `rtl.css` stylesheet.


### Translations

The translations live in the `lib/translations` folder. There are currently [43 language translations](https://github.com/altea-software/pickadate-accessible/tree/master/lib/translations) included.


## Accessibility & Compatibility

This library is fully compliant with WCAG 2.1 AA standards, providing:

- **Enhanced keyboard navigation** with proper focus management and tab order
- **Screen reader compatibility** with ARIA labels and announcements
- **Strict equality compliance** for improved maintainability and reliability
- **Improved color contrast** meeting AA standards
- **Better focus indicators** for keyboard users

The accessibility improvements ensure that the date and time pickers are usable by people with disabilities, including those who rely on screen readers or keyboard navigation.

### What's New in This Fork

This accessible fork includes significant improvements over the original library:

**Accessibility Enhancements:**
- Full WCAG 2.1 AA compliance implementation
- Enhanced keyboard navigation with proper focus management
- Screen reader compatibility with ARIA labels and announcements
- Improved color contrast meeting AA standards
- Better focus indicators for keyboard users

**jQuery Compatibility:**
- **Replaced `jQuery.isArray()`** with native `Array.isArray()` - 32 occurrences updated across all picker files
- **Eliminates jQuery migrate warnings** when using jQuery 3.7.1+ with the migrate plugin
- **Modern browser support** - IE9+ and all modern browsers
- **Future-proof** for upcoming jQuery versions where deprecated functions will be removed



<br>

## Building with Grunt

[Grunt](http://gruntjs.com/) `~0.4.5` is used to build the project files. To get started, clone the project and then run:

- `npm install` to get the required node modules.
- `grunt test --verbose` to confirm you have all the dependencies.


Type out `grunt --help` to see a list of all the tasks available. The generally used tasks are:

- `grunt develop` compiles the LESS files and watches for any source changes.
- `grunt package` compiles and then minifies the source files.
- `grunt test` tests the entire package.




<br>

<a name="less-styling"></a>
## Styling with LESS

The picker themes are built using [LESS](http://lesscss.org/) with Grunt. To customize the CSS output, read the `_variables.less` file in the `lib/themes-source` folder. You can specify:

- colors for the theme,
- sizes for the picker,
- media-query breakpoints,
- and a whole bunch of other stuff.


Make sure to run the `grunt develop` task before making any changes to compile it into CSS.





<br>

## Bugs

Before opening a new issue, please search the existing [Issues](https://github.com/altea-software/pickadate-accessible/issues) for anything similar – there might already be an answer to your problem. You might also wanna check out the [Contributing](https://github.com/altea-software/pickadate-accessible/blob/master/CONTRIBUTING.md) guide.





<br>

## Contributing

Before contributing any code to the project, please take a look at the [Contributing](https://github.com/altea-software/pickadate-accessible/blob/master/CONTRIBUTING.md) guide.

If there’s anything you’d like to discuss, we like to hang out on Spectrum.


[![Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/pickadate)





<br>

## Support

If you find this library useful and would like to see further development, consider [supporting it](http://selz.co/1g80kCZ).





<br><br>

---

© 2014 [Amsul](http://twitter.com/amsul_)

Licensed under [MIT](http://amsul.ca/MIT)
