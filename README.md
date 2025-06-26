# CleanUI

# What, why, how?
CleanUI is a huge and utterly complex scss package that provides me my basic styles for my projects.
Feel free to use it, but please do not copy it and claim it as your own.
```npm
npm install @kablan/clean-ui --save
```
# Usage
### SCSS
Import the SCSS entry point in your main SCSS file.
You can optionally override the default variables in `/scss/_variables.scss` before importing the styles.
```scss
// Optionally override default variables from /scss/_variables.scss
$primary: #ff00ff;

// Import the CleanUI styles
@use "@kablan/clean-ui/scss/index" as *;
```

### CSS
If you do not use SCSS, you can include the precompiled CSS directly in your HTML or via import.
```html
<link rel="stylesheet" href="node_modules/@kablan/clean-ui/css/index.css">
```
```js
import '@kablan/clean-ui/css/index.css';
```

<hr />

* SCSS: Allows variable ovverides and tree-shaking via `@use`.
* CSS: Precompiled version for direct use without SCSS processing. Though, no variable overrides are possible.

_See [_variables](scss/_variables.scss)_ for all available variables._
