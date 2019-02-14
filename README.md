## Boilerplate Drupal theme with a modern development workflow

### Quick start
* Run `yarn` from the theme directory to install dependencies
* Copy the `.env.example to` file to a `.env` file:
  * Edit `DEV_URL`. It should reflect your local development hostname
* `yarn start` — Compile assets when file changes are made, start Browsersync session
* `yarn build` — Compile and optimize the files in your src directory for production


### Features
* Sass
* Modern JavaScript or TypeScript
* ESLint - extends [airbnb-base](https://www.npmjs.com/package/eslint-config-airbnb-base) 
* Stylelint - extends [stylelint-config-airbnb](https://www.npmjs.com/package/stylelint-config-airbnb) 
* Critical CSS - [postcss-critical-css](https://github.com/zgreen/postcss-critical-css)
* [Husky](https://github.com/typicode/husky) - Git hooks made easy, e.g. linting staged files before commit
* [Parceljs](https://parceljs.org//) - Blazing fast, zero configuration web application bundler
* [Browsersync](http://www.browsersync.io/) - Synchronized browser testing
* [sanitize.css](https://github.com/csstools/sanitize.css) - A best-practices CSS foundation


### Requirements
Make sure all dependencies have been installed before moving on:


* [Drupal](https://www.drupal.org//) > 8.x
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
│   ├── base
│   ├── components
│   ├── main.js
│   ├── main.scss
│   ├── mixins
│   └── settings
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
