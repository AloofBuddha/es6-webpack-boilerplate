# Boilerplate project for ES6 (Babel) and Webpack

Boilerplate for building ES6 web apps.

## Getting Started

1. `npm install`
2. `npm start`

### NPM Tasks

- `npm start` runs Webpack's development server (watches for file changes and reloads your browser)
- `npm run compile` compiles your app for production (minify and optimizes the hell out of your code)
- `npm test` runs lints and tests (currently, there are no tests)
  - `npm run lint` lints your code using [ESLint](eslint.org) (OBEY ESLINT!)

### Vendor Module Packaging

Webpack's [CommonsChunkPlugin](http://webpack.github.io/docs/list-of-plugins.html#commonschunkplugin) is used to split your code and vendor dependencies into separate bundles. Ideally, that allows you to cache dependency code longer than application code and allows you to easily blackbox dependency code when debugging.

To add dependencies to your _vendor_ bundle, just edit `src/vendor.js`.

## Technology

- Webpack to package JS code and assets
- Babel.js to compile modern JS to ES5
