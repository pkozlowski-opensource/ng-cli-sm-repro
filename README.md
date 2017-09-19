# ng-cli-sm-repro

To reproduce:
* clone this repo
* `npm install`
* `ng build --prod --build-optimizer --sourcemap`
* `source-map-explorer ./dist/main.7b9d31ed86b1018dfaed.bundle.js`

This results in the following error:

> Your source map only contains one source ( webpack:///main.7b9d31ed86b1018dfaed.bundle.js )
  This typically means that your source map doesn't map all the way back to the original sources.
  This can happen if you use browserify+uglifyjs, for example, and don't set the --in-source-map flag to uglify.
  See  https://github.com/danvk/source-map-explorer/blob/master/README.md#generating-source-maps
