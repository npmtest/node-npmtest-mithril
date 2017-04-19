# npmtest-mithril

#### test coverage for  [mithril (v1.1.1)](https://github.com/lhorie/mithril.js#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-mithril.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-mithril) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-mithril.svg)](https://travis-ci.org/npmtest/node-npmtest-mithril)

#### A framework for building brilliant applications

[![NPM](https://nodei.co/npm/mithril.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mithril)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-mithril/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-mithril/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-mithril/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-mithril/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-mithril/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-mithril/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-mithril/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-mithril/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-mithril/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-mithril/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-mithril/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-mithril/build/test-report.html](https://npmtest.github.io/node-npmtest-mithril/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-mithril/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-mithril/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-mithril/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mithril/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mithril/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mithril/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-mithril/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-mithril/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Leo Horie"
    },
    "bin": {
        "ospec": "./ospec/bin/ospec",
        "bundle": "./bundler/bin/bundle"
    },
    "bugs": {
        "url": "https://github.com/lhorie/mithril.js/issues"
    },
    "dependencies": {},
    "description": "A framework for building brilliant applications",
    "devDependencies": {
        "eslint": "^3.16.1",
        "istanbul": "^0.4.3",
        "marked": "^0.3.6"
    },
    "directories": {},
    "dist": {
        "shasum": "0c98644c90503eec2187f66a851ba4053c4a5d66",
        "tarball": "https://registry.npmjs.org/mithril/-/mithril-1.1.1.tgz"
    },
    "gitHead": "8a7f2f85d75f0e86d4e33c0cc0bcc072f046a2b0",
    "homepage": "https://github.com/lhorie/mithril.js#readme",
    "license": "MIT",
    "main": "mithril.js",
    "maintainers": [
        {
            "name": "lhorie"
        },
        {
            "name": "tivac"
        }
    ],
    "name": "mithril",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/lhorie/mithril.js.git"
    },
    "scripts": {
        "build": "npm run build-browser & npm run build-min",
        "build-browser": "node bundler/cli browser.js -o mithril.js",
        "build-min": "node bundler/cli browser.js -o mithril.min.js -m",
        "cover": "istanbul cover --print both ospec/bin/ospec",
        "dev": "node bundler/cli browser.js -o mithril.js -w",
        "gendocs": "node docs/generate",
        "lint": "eslint .",
        "lint:fix": "eslint . --fix",
        "lintdocs": "node docs/lint",
        "posttest": "npm run lint || true",
        "postversion": "git push --follow-tags",
        "preversion": "npm run test",
        "release": "npm version -m \"v%s\"",
        "test": "node ospec/bin/ospec",
        "version": "npm run build && git add mithril.js mithril.min.js"
    },
    "version": "1.1.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
