# \<saiku-embed\>

> A web component to embed Saiku Analytics using [Polymer](https://www.polymer-project.org/).

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/OSBI/saiku-embed-element)

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

    <!-- Polyfill Web Components support for older browsers -->
    <script src="./bower_components/webcomponentsjs/webcomponents-lite.js"></script>

    <!-- Import element -->
    <link rel="import" href="./bower_components/saiku-embed/saiku-embed.html">
  </head>
  <body>

    <!-- Use element -->
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
`schema`                     | *String*                                                                                                   |         | Schema name. e.g: `FoodMart`
`cube`                       | *String*                                                                                                   |         | Cube name. e.g: `Sales`
`default_mdx_filter`         | *String*                                                                                                   |         | Extend `default_mdx_filter` to add level to filter axis.
`default_mdx_filter_rows`    | *String*                                                                                                   |         | Extend `default_mdx_filter_rows` to add level to rows axis.
`default_mdx_filter_columns` | *String*                                                                                                   |         | Extend `default_mdx_filter_columns` to add level to columns axis.
`lang`                       | `cn`, `cs`, `de`, `en`, `es`, `fi`, `fr`, `hr`, `hu`, `it`, `ja`, `ko`, `lt`, `nb`, `nl`, `pl`, `pt`, `ru` |         | Specifies the language to be used.
`mode`                       | `view`, `edit`, `table`, `chart`, `map`                                                                    |         | Specifies the mode to use when opening a Saiku file.
`path_file_saiku`            | *String*                                                                                                   |         | The path of your Saiku file. e.g: `/homes/home:admin/example.saiku`
`splash`                     | *Boolean*                                                                                                  | `true`  | Enable or disable splash screen.
`plugin`                     | *Boolean*                                                                                                  | `false` | Work in plugin mode.
`hide_workspace_icons`       | *Boolean*                                                                                                  | `false` | Hide some icons on Saiku Toolbar.
`show_help`                  | *Boolean*                                                                                                  | `false` | Show help using [intro.js](http://introjs.com/).

## Development

In order to run it locally you'll need to fetch some dependencies.

1. Install [Bower](http://bower.io/) & [Polymer CLI](https://www.npmjs.com/package/polymer-cli):

    ```sh
    $ [sudo] npm install -g bower polymer-cli
    ```

2. Install local dependencies:

    ```sh
    $ bower install
    ```

3. To test the project, start the development server and open `http://localhost:8081`.

    ```sh
    $ polymer serve
    ```

## Browser Support

![Chrome](https://raw.github.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) |
![Firefox](https://raw.github.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) |
![Edge](https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png) |
![Safari](https://raw.github.com/alrra/browser-logos/master/src/safari/safari_48x48.png) |
![Opera](https://raw.github.com/alrra/browser-logos/master/src/opera/opera_48x48.png)
--- | --- | --- | --- | --- |
Chrome or Chromium version 49 or later ✔ | Firefox 51 or later ✔ | Edge 15.15063 or later ✔ | Safari or Mobile Safari 10 or later ✔ | Opera 36 or later ✔ |

## Contributing

If you want to help, please read the [Contributing](https://github.com/OSBI/saiku-embed-element/blob/master/CONTRIBUTING.md) guide.

## History

For detailed changelog, see [Releases](https://github.com/OSBI/saiku-embed-element/releases).

## License

[Apache License Version 2](https://github.com/OSBI/saiku_community_website/blob/master/LICENSE) © [Meteorite BI](http://www.meteorite.bi/)
