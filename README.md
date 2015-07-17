# Stencil Utilities

CSS utilities for mobile browsers.

Stencil Utilities provide common CSS patterns that can be used in various one-off situations to affect appearance or spacing.


## Available Utilities

* [Dimension](https://github.com/mobify/stencil-utils/tree/master/dist/dimension)
* [Layout](https://github.com/mobify/stencil-utils/tree/master/dist/layout)
* [Spacing](https://github.com/mobify/stencil-utils/tree/master/dist/spacing)
* [Text](https://github.com/mobify/stencil-utils/tree/master/dist/text)
* [Visibility](https://github.com/mobify/stencil-utils/tree/master/dist/visibility)


## Requirements

- [Sass](http://sass-lang.com/) 3.4+
- [Grunt](http://gruntjs.com/)
- Adaptive.js 2.1 +

## Installation

Install with [Grunt](http://gruntjs.com/):

```
grunt component:install:utils
```

Once installed, the Stencil Utilities live in your project’s `app/bower_components` directory. Individual utilities will provide a stylesheet, including example markup and (optionally) JavaScript. To learn more, visit the [dev centre documentaton](#).


## Using a Stencil Utility

Utility classes are conceptually a bit like a Sass mixin; they allow you to add new style rules to an existing component, except that they are applied as classes in your markup. An example utility class is `.u-width-full`. It does exactly what it says: make an element expand to fill the full width of its container.

Use these utilities in conjunction with other components for building layout (e.g. a Grid component and `.u-width-full`), or apply them to elements on your page in place of custom modifiers (e.g.: `.c-button.u-width-full` to make a button full-width without having to create a modifier).

Once your theming is in place, and you've built any custom components you need, you'll find you can build full pages simply by writing HTML, applying utility classes to apply one-off modifications to page elements.

Some things to note about utility classes:

1. Utility classes should apply a focused set of CSS properties that are applicable across a wide range of components;
2. Utility classes use a `.u-` prefix instead of the `.c-` prefix used for a component’s class name;
3. Utility classes almost always use `!important` in their styles. This is to ensure their styles always apply on top of other styles. Use utiliy classes surgically to adjust existing components, and use with care.


## Previewing Utilities

1. If you have Sass < 3.4, run `gem update sass`. If you don't have Bower installed, run `npm install -g bower`.

2. In your utilities directory, run `npm install && bower install`.

3. Run `grunt serve` to run testing environment locally. It will automatically recompile your stylesheets when you change them.

4. Navigate to `localhost:3000`.

5. Utilities are found in `tests/visual/ directory`.

Learn about setting up and running Stencil tests in our [dev centre documentation](#).


## Learn More

To learn more about Utilities, Stencil, and Stencil Components, visit our dev centre documentation:

[Use a Component](#)
[Tips and Recommendations](#)
[Uninstall a Component](#)


## License

*MIT License. Stencil is Copyright © 2014 Mobify. It is free software and may be redistributed under the terms specified in the LICENSE file.*
