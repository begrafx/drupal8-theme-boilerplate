## Boilerplate Drupal theme with a modern development workflow

### Features
* Sass
* Modern JavaScript
* ESLint - extends [airbnb-base](https://www.npmjs.com/package/eslint-config-airbnb-base) 
* Stylelint - extends [stylelint-config-airbnb](https://www.npmjs.com/package/stylelint-config-airbnb) 
* Critical CSS - [postcss-critical-css](https://github.com/zgreen/postcss-critical-css)
* [Parceljs](https://parceljs.org//) for compiling assets, optimizing images, and concatenating and minifying files
* [Browsersync](http://www.browsersync.io/) for synchronized browser testing


### Requirements
Make sure all dependencies have been installed before moving on:

* [Drupal](https://www.drupal.org//) > 8.x
* [PHP](https://secure.php.net/manual/en/install.php) >= 7.1.3
* [Composer](https://getcomposer.org/download/)
* [Node.js](http://nodejs.org/) >= 8.0.0
* [Yarn](https://yarnpkg.com/en/docs/install)
* [Link CSS](https://www.drupal.org/project/link_css) - Drupal module needs to be enabled in development for Hot Module Reloading


### Theme installation

### Theme structure

```shell
├── README.md
├── boilerplate.info.yml
├── boilerplate.libraries.yml
├── config
│   └── bs-config.js
├── package.json
├── public
│   ├── favicons
│   ├── fonts
│   └── icons
├── src
│   ├── abstractions
│   ├── assets
│   ├── base
│   ├── components
│   ├── main.js
│   ├── main.scss
│   ├── mixins
│   ├── settings
│   └── someModule.js
├── templates
│   ├── block
│   ├── content
│   ├── layout
│   ├── paragraphs
│   └── partials
├── yarn-error.log
└── yarn.lock
```

Drupal Paragraph components should go into `src/components` directory:
```shell
src
├── components
    ├── README.md
    ├── accordion
    │   ├── accordion.js
    │   └── accordion.scss
    └── simple-product
        ├── simple-product.scss
        └── simpleProduct.js
```

### Theme setup

### Theme development

* Run `yarn` from the theme directory to install dependencies
* Copy the `.env.example to` file to a `.env` file:
  * `DEV_URL` should reflect your local development hostname

### Build commands

* `yarn start` — Compile assets when file changes are made, start Browsersync session
* `yarn build` — Compile and optimize the files in your src directory for production
