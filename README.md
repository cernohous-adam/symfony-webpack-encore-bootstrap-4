# symfony-webpack-encore-bootstrap-4

- yarn add @symfony/webpack-encore --dev

- yarn add jquery --dev
- yarn add bootstrap@4.0.0-beta.2

*Many of Bootstrap 4 components require the use of JavaScript to function. Specifically, they require jQuery, [Popper.js](https://popper.js.org/), and Bootstrap own JavaScript plugins. jQuery must come first, then Popper.js, and then our JavaScript plugins.*

So its necessary to require bootstrap.bundle.js instead of bootstrap.js in your main JS file due to Popper dependency.

```
require('bootstrap/dist/js/bootstrap.bundle.js');
```
See the [example file](js/frontend.js)
