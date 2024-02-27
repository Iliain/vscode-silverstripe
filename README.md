# Silverstripe

Provides [SilverStripe](http://www.silverstripe.org/) syntax highlighting and snippets.

[![Powered by Sanchez](https://raw.githubusercontent.com/gorriecoe/silverstripe-sanchez/master/resources/poweredby.png)](https://github.com/gorriecoe/silverstripe-sanchez)

## Bug Fix Note

This version currently fixes the issue with `.silverstripe_sanchez` files not being located and loaded (which allows for custom snippets). Until this is merged into the main repository, you can use this version.

* Use node 14
* Run `npm install`
* Run `npm run vscode:prepublish`
* Copy the dist files to the dist folder of your existing extension (e.g. `~/.vscode/extensions/adrianhumphreys.silverstripe-1.0.6/dist/`)
* Restart VSCode if open, fix should take effect

## Features

- Reads the project composer.lock file to determine the available snippets.
- Php snippets follow [psr-2 standards](http://www.php-fig.org/psr/psr-2/)
- Snippets inject use item if available and possible.
- Supports 4.\* and 3.\*.
- Uses full word prefixes so you don't have to remember abbreviations.
- Includes snippets for addons modules such as [tagfield](https://github.com/silverstripe/silverstripe-tagfield) and [linkable](https://github.com/sheadawson/silverstripe-linkable).
- .ss templates include scope and conditional indentation.
- .ss templates support go to definition for `<% include %>`, `<% themedCSS %>` and `<% themeJavascript %>`.
- .ss templates autocomplete paths include, themedCSS and themeJavascript. ie. includepagination will complete to `<% include SilverStripe/Blog/Pagination %>` if found in the appropriate directory.

## Options

[Add your own snippets](https://github.com/gorriecoe/silverstripe-sanchez)

## Enable emmet

Open `Preferences` -> `Settings`

Add below settings to enable Emmet for .ss files:

```json
"emmet.includeLanguages": {
    "silverstripe": "html"
}
```

## Contributions

Go for gold, if it adds value, add it and I'll merge it.


