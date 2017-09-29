# \<saiku-embed\>

> A web component to embed Saiku Analytics using [Polymer](https://www.polymer-project.org/).

## Install

Install the component using [Bower](https://bower.io/):

```sh
$ bower install saiku-embed --save
```

Or [download as ZIP](https://github.com/OSBI/saiku-embed-element/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="./bower_components/webcomponentsjs/webcomponents-lite.js"></script>
    ```

2. Import Element:

    ```html
    <link rel="import" href="./bower_components/saiku-embed/saiku-embed.html">
    ```

3. Start using it!

    ```html
    <saiku-embed url="http://localhost:8080/" username="admin" password="admin"></saiku-embed>
    ```

Here's an example of basic usage:

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, minimum-scale=1, initial-scale=1, user-scalable=yes">
    <title>saiku-embed demo</title>
    <script src="./bower_components/webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="./bower_components/saiku-embed/saiku-embed.html">
  </head>
  <body>
    <saiku-embed url="http://localhost:8080/" username="admin" password="admin"></saiku-embed>
  </body>
</html>
```

## Options

Attribute                    | Options                                                                                                    | Default | Description
---                          | :---:                                                                                                      | :---:   | ---
`url`                        | *String*                                                                                                   |         | Saiku's URL (**Required**).
`username`                   | *String*                                                                                                   |         | User name to access Saiku.
`password`                   | *String*                                                                                                   |         | Password to access Saiku.
`width`                      | *String*                                                                                                   | `800`   | The `width` attribute specifies the width of an `<saiku-embed>`, in pixels.
`height`                     | *String*                                                                                                   | `600`   | The `height` attribute specifies the height of an `<saiku-embed>`, in pixels.
`schema`                     | *String*                                                                                                   |         | Schema name. `e.g: FoodMart`
`cube`                       | *String*                                                                                                   |         | Cube name. `e.g: Sales`
`default_mdx_filter`         | *String*                                                                                                   |         |
`default_mdx_filter_rows`    | *String*                                                                                                   |         |
`default_mdx_filter_columns` | *String*                                                                                                   |         |
`lang`                       | `cn`, `cs`, `de`, `en`, `es`, `fi`, `fr`, `hr`, `hu`, `it`, `ja`, `ko`, `lt`, `nb`, `nl`, `pl`, `pt`, `ru` |         | Specifies the language to be used.
`mode`                       | `view`, `edit`, `table`, `chart`, `map`                                                                    |         | Specifies the mode to use when opening a Saiku file.
`path_file_saiku`            | *String*                                                                                                   |         | The path of your Saiku file. `/homes/home:admin/example.saiku`
`splash`                     | *Boolean*                                                                                                  | `true`  | Enable or disable splash screen.
`plugin`                     | *Boolean*                                                                                                  | `false` | Work in plugin mode.
`hide_workspace_icons`       | *Boolean*                                                                                                  | `false` | Hide some icons on Saiku Toolbar.
`show_help`                  | *Boolean*                                                                                                  | `false` | Show help using [intro.js](http://introjs.com/).

## Browser Support

![Chrome](https://raw.github.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) |
![Firefox](https://raw.github.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) |
![Edge](https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png) |
![Safari](https://raw.github.com/alrra/browser-logos/master/src/safari/safari_48x48.png) |
![Opera](https://raw.github.com/alrra/browser-logos/master/src/opera/opera_48x48.png)
--- | --- | --- | --- | --- |
Chrome or Chromium version 49 or later ✔ | Firefox 51 or later ✔ | Edge 15.15063 or later ✔ | Safari or Mobile Safari 10 or later ✔ | Opera 36 or later ✔ |

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

## Contributing

If you want to help, please read the [Contributing](https://github.com/OSBI/saiku-embed-element/blob/master/CONTRIBUTING.md) guide.

## History

For detailed changelog, see [Releases](https://github.com/OSBI/saiku-embed-element/releases).

## License

[Apache License Version 2](https://github.com/OSBI/saiku-embed-element/blob/master/LICENSE) © Meteorite BI
