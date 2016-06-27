# solint

[![NPM version](http://img.shields.io/npm/v/solint.svg)](https://www.npmjs.org/package/solint) [![Build status](https://ci.appveyor.com/api/projects/status/wwajr0886e00g8je/branch/master?svg=true)](https://ci.appveyor.com/project/weifund/solint/branch/master) [![Coverage Status](https://coveralls.io/repos/github/weifund/solint/badge.svg?branch=master)](https://coveralls.io/github/weifund/solint?branch=master) [![NPM Downloads](https://img.shields.io/npm/dm/solint.svg)](https://www.npmjs.org/package/solint)

A mighty, modern Solidity linter that helps you enforce consistent conventions and avoid errors in your Solidity smart-contracts.

Note, this module is still under heavy development.

## Install

```
npm install --save-dev solint
```

## Planned Design

```
solint contracts/**/*.sol
```

which results in something like:

```
START:
27 06 2016 13:11:29.782:INFO [solint]: Solint v0.1.0
ERROR: 'Do not use the `new` term in method input variable names'
  function set(uint _newValue...
    X input uses `new` term
```

rules can be set and applied in a `.solint` file.

## About

The idea behind solint is to provide a first pass at linting Solidity smart-contracts. There is an utter lack of these tools available in the ecosystem and we should all work together to build great tools that can catch very dangerous bugs or bad practices.

Linting is one of the first lines of defence against things like the DAO attack. It is absolutely imperative linting standards and utilities be developed to help developers build better and safer smart-contracts.

## Contributing

Please help better the ecosystem by submitting issues and pull requests to solint. We need all the help we can get to build the absolute best linting standards and utilities. We follow the AirBNB linting standard. Please read more about contributing to `solint` in the `CONTRIBUTING.md`.

## Guides

You'll find more detailed information on using solint and tailoring it to your needs in our guides:

- [User guide](docs/user-guide.md) - Usage, configuration, FAQ and complementary tools.
- [Developer guide](docs/developer-guide.md) - Contributing to solint and writing your own plugins & formatters.

## Help out

There is always a lot of work to do, and will have many rules to maintain. So please help out in any way that you can:

- Create, enhance, and debug rules (see our guide to ["Working on rules"](CONTRIBUTING.md)).
- Improve documentation.
- Chime in on any open issue or pull request.
- Open new issues about your ideas for making stylelint better, and pull requests to show us how your idea works.
- Add new tests to *absolutely anything*.
- Work on [improving performance of rules](docs/developer-guide/benchmarks.md).
- Create or contribute to ecosystem tools, like the plugins for Atom and Sublime Text.
- Spread the word.

Please consult our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing](CONTRIBUTING.md) docs before helping out.

We communicate via [issues](https://github.com/weifund/solint/issues) and [pull requests](https://github.com/weifund/solint/pulls).

There will also [stackoverflow](http://stackoverflow.com/questions/tagged/solint), which is our preferred QA forum. Tag your post with "solint".

## Important documents

- [Changelog](CHANGELOG.md)
- [Contributing Guidelines](CONTRIBUTING.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [License](https://raw.githubusercontent.com/weifund/solint/master/LICENSE)

## Licence

```
The MIT License

Copyright (c) 2015 WeiFund. www.weifund.io

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
