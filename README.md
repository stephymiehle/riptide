# Riptide

![Screenshot of Riptide theme](screenshot.png?raw=true)

Riptide is a colorful and dark theme for Textual IRC.

Riptide is based on [emilyst/Eighties-Aligned](https://github.com/emilyst/Eighties-Aligned), "a Textual 5 style which derives elements of its appearance from the 'Tomorrow Night Eighties' the 'Nox' themes included with the Textual IRC client." The color scheme is borrowed (with love) from [voronianski/oceanic-next-color-scheme](https://github.com/voronianski/oceanic-next-color-scheme) and also includes a few favorites from [base16](https://chriskempson.github.io/base16/).

Nick, timestamp, and font preferences are all respected; this theme will not override them.

To make customization easy, this theme uses Sass. The compiled CSS file is included for those who want to use the theme as-is, but if you want to remix this in any way, I encourage you to edit `design.scss` and the `Data/Resources/scss` directory, then watch for changes with the compiler of your choice (I used compass and the `config.rb` is included).

## Icons

### Adding Icons

Icons are added from [Fontello](http://fontello.com/); only a limited set is included. Visit Fontello and load the provided config file to import the included set. If you want to add or remove icons, generate a new set, replace the font files in `Data/Resources/riptide-icons`, and copy the contents of `(your Fontello download)/css/riptide-icons-codes.css` to `Data/Resources/scss/riptide-icons.scss`.

### Referencing Icons in SCSS

A mixin is included in `riptide-icons.scss`. Using a selector with `:before` or `:after`, add the following:

    @include icon(icon-name);

Of course, replace "icon-name" with the icon you want to use. The icon name **must** be in `riptide-icons.scss` to work.

# Installing Riptide

1. Download the Riptide theme

2. Open textual://custom-styles-folder and unarchive the theme; feel free to rename the directory if you like.

3. Open Textual and navigate to Preferences ➜ Style. Select "Riptide" from the dropdown.

4. Enjoy!
