*This is useful if you want to test React components in Mocha.*

The things you will need to take in order to do this:

1. The Mocha.opts provides the default options for Mocha > It needs to know that the tests will contain ES6 and JSX elements, so needs to be aware to transpile them using Babel.
2. The .babelrc has the relevant entries to trasnpile both ES6 and JSX elements.
3. The package.json contains all of the relevant modules. Be sure to install any that are not already in your project.
4. The package.json also contains the `test` and `test:watch` script entries that you will also want.
5. Each component, as required, can then have a test. Mocha is basically going to look for any file with the naming structure `<something>-test.js`, so you can structure and name your tests whatever makes sense, but typically you want to name them the same as the component it tests, and maybe always have them in a `_tests` directory (as this repository is laid out).
