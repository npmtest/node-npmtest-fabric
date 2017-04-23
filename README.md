# npmtest-fabric

#### basic test coverage for  [fabric (v2.0.0-beta.1)](http://fabricjs.com/)  [![npm package](https://img.shields.io/npm/v/npmtest-fabric.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-fabric) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-fabric.svg)](https://travis-ci.org/npmtest/node-npmtest-fabric)

#### Object model for HTML5 canvas, and SVG-to-canvas parser. Backed by jsdom and node-canvas.

[![NPM](https://nodei.co/npm/fabric.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/fabric)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-fabric/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-fabric/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-fabric/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-fabric/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-fabric/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-fabric/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-fabric/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-fabric/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-fabric/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-fabric/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-fabric/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-fabric/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-fabric/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-fabric/build/test-report.html](https://npmtest.github.io/node-npmtest-fabric/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-fabric/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-fabric/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-fabric/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-fabric/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fabric/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fabric/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-fabric/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-fabric/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Juriy Zaytsev"
    },
    "browser": {
        "canvas": false,
        "fs": false,
        "jsdom": false,
        "xmldom": false
    },
    "bugs": {
        "url": "https://github.com/kangax/fabric.js/issues"
    },
    "contributors": [
        {
            "name": "Andrea Bogazzi"
        }
    ],
    "dependencies": {
        "canvas-prebuilt": "1.6.5-prerelease.1",
        "jsdom": "9.x.x",
        "xmldom": "0.1.x"
    },
    "description": "Object model for HTML5 canvas, and SVG-to-canvas parser. Backed by jsdom and node-canvas.",
    "devDependencies": {
        "eslint": "2.x.x",
        "istanbul": "0.4.x",
        "onchange": "^3.0.2",
        "qunit": "0.9.x",
        "uglify-js": "2.7.x"
    },
    "directories": {},
    "dist": {
        "shasum": "5f9a3448feef32b1bad6fd7c99b8ff28f006ba14",
        "tarball": "https://registry.npmjs.org/fabric/-/fabric-2.0.0-beta.1.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "879d5b4e669d04141fa574ad452d08faf4165d74",
    "homepage": "http://fabricjs.com/",
    "keywords": [
        "canvas",
        "graphic",
        "graphics",
        "SVG",
        "node-canvas",
        "parser",
        "HTML5",
        "object model"
    ],
    "license": "MIT",
    "main": "./dist/fabric.js",
    "maintainers": [
        {
            "name": "asturur"
        },
        {
            "name": "kangax"
        }
    ],
    "name": "fabric",
    "optionalDependencies": {
        "canvas-prebuilt": "1.6.5-prerelease.1",
        "jsdom": "9.x.x",
        "xmldom": "0.1.x"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kangax/fabric.js.git"
    },
    "scripts": {
        "all": "npm run build && npm run test && npm run lint && npm run lint_tests && npm run export_dist_to_site && npm run export_tests_to_site",
        "build": "node build.js modules=ALL exclude=json,gestures",
        "build:watch": "onchange 'src/**/**' 'test/**/**' 'HEADER.js' 'lib/**/**' -- npm run build_export",
        "build_export": "npm run build && npm run export_dist_to_site",
        "build_with_gestures": "node build.js modules=ALL exclude=json",
        "export_dist_to_site": "cp dist/fabric.js ../fabricjs.com/lib/fabric.js && cp -r src HEADER.js lib ../fabricjs.com/build/files/",
        "export_tests_to_site": "cp test/unit/*.js ../fabricjs.com/test/unit",
        "lint": "eslint --config .eslintrc.json src",
        "lint_tests": "eslint test/unit --config .eslintrc_tests",
        "test": "node test.js"
    },
    "version": "2.0.0-beta.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
