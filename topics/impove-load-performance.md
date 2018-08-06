## Optimize The Angular 2 Application For Better Performance?

### compressed images.
### minify css
### minify js.
### I use async on my scripts.
### scripts shoild be yours avoid including extra and unwanted packages
### The scripts are around 700kb
### google speed test
### minified version of the libs I use e.g. bootstrap etc.

###  angular seed
angular seed provide following feature

- [x] Production and development builds.

- [x] Ahead-of-Time compilation support.

- [ ] Uses codelyzer for static code analysis, which verifies that the project follows practices from 
    the Angular style guide.

- [x] Tree-Shaking production builds with Rollup.

- [x] Sample unit tests with Jasmine and Karma including code coverage via istanbul.

- [x] End-to-end tests with Cypress.

- [x] Development server with Livereload.

- [x] Provides full Docker support for both development and production environment
    Support for Angular Mobile Toolkit

- [ ] Allows you to analyze the space usage of created bundles by using source-map-explorer
    Ready to go, statically typed build system using gulp for working with TypeScript.

##        OR

    I would consider the following points while optimizing the angular 2 app:
            Consider AOT compilation.
            Application is bundled, uglified, and tree shaking should be done.
            Application doesn’t have un-necessary import statements.
            Any 3rd party library, which is not used, is removed from the application.
            Have all dependencies and dev-dependencies are clearly separated.
            Consider lazy loading instead of fully bundled app if the app size is more.