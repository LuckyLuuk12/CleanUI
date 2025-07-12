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

// Import the CleanUI styles and partials
@use '@kablan/clean-ui/scss/_imports.scss' as imports;
@use '@kablan/clean-ui/scss/_utils.scss' as utils;
@use '@kablan/clean-ui/scss/_variables.scss' as *;
@use '@kablan/clean-ui/scss/_interactable.scss' as *;
@use '@kablan/clean-ui/scss/_containers.scss' as *;
@use '@kablan/clean-ui/scss/_layout.scss' as *;
@use '@kablan/clean-ui/scss/_highlight.scss' as *;
@use '@kablan/clean-ui/scss/index.scss' as *;
```

### CSS
If you do not use SCSS, you can include the precompiled CSS directly in your HTML or via import by using the CDN
from cloudflare:
```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/clean-ui/1.0.0/css/index.css">
```
```js
import '@kablan/clean-ui/css/index.css';
```

### Code Highlighting
This package also includes a color theme for [Highlight.js](https://highlightjs.org/).
To use it, make sure you import Highlight.js in your project as well, e.g.:
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.11.1/highlight.min.js"></script>
<script> hljs.highlightAll(); </script>
```

<hr />

* SCSS: Allows variable overrides and tree-shaking via `@use`.
* CSS: Precompiled version for direct use without SCSS processing. Though, no variable overrides are possible.

_See [_variables](scss/_variables.scss)_ for all available variables._
