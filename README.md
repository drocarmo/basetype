# Basetype

An eloquently modular typographic scale tool using Sass.

## Components

#### _settings.scss
> Using Sass `$maps`, this is where you put your typeface settings you are using for your project. Think of it as your `_data` directory in [Jekyll](http://jekyllrb.com/docs/datafiles/). It won't ever appear in your production code, it's there for data reference for when you pass in your functions/mixins.

#### _functions.scss
> Functions/mixins that contain the magic from [The Ultimate Package](https://github.com/ultimate-package/tools.font-scale).

## Example

```scss

// Your project's Sass

@import "settings";
@import "functions";

h1 {
  font-family: font-family($font-opensans);
  @include font-scale(large);
}

// CSS output

h1 {
  font-family: Open Sans, sans-serif;
  font-size: 36px;
  line-height: 42px;
}
```

==============================

Again, props to [The Ultimate Package](https://github.com/ultimate-package/tools.font-scale) for the mixin magic. Make sure to include and `@import` the two partials into your new project and you're good to go. Let me know if you have any questions.
