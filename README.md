Raw SVG icons for RPG-Awesome
=============================

These are the raw SVG files used to generate new font files for [RPG Awesome](https://github.com/nagoshiashumari/Rpg-Awesome).


# Adding New Icons

First, add the new SVG file to `/Font`.

Next, use [IcoMoon](https://icomoon.io/app/) to import all of the SVG files located in `/Font`.

Once imported, proceed to the next section "Download". Set your preferences to the following:

* Font Name: `rpgawesome-webfont`
* Class Prefix: `ra-var-icon`
* Include Metadata in Fonts: true
* Generate Stylesheet Variables for: Sass
* Metadata URL: `https://github.com/nagoshiashumari/Rpg-Awesome/`
* Metadata License: `MIT`

Without these changes, the font file will be rejected when issuing a pull request to RPG Awesome.

Once the Preferences are set, click Download. You will receive a ZIP file. In it, the important files you will need to copy over to the RPG Awesome repo are:

* `zip/fonts` => `rpg-awesome/fonts`

You will need to manually copy and paste `zip/variables.scss` into `rpg-awesome/scss/_variables.scss`, overwritting the old `ra-var-icon` variables.
