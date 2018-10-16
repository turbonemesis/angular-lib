
[![Circle CI Badge][circleci-badge]][circleci-link]
[![codecov][codecov-image]][codecov-link]
[![Dependency Status][dependency-image]][dependency-link]
[![Dev Dependency Status][dev-dependency-image]][dev-dependency-link]
[![Peer Dependency Status][peer-dependency-image]][peer-dependency-link]
[![NPM Downloads][npm-downloads-image]][npm-downloads-link]
[![NPM Version][npm-version-image]][npm-version-link]
[![MIT License][npm-license-image]][npm-license-link]

# @rd/core [![Public or Private Repo][public-true-image]][public-true-link]

## Getting Started

First, `git clone git@github.com:RentDynamics/ng-core.git` into its own directory

Next, `cd ./<package_name>` (into the cloned directory)

After that, `npm i`

At this point, you should be able to run `ng b`, which will use ng-packagr to package the library into the `./dist/<package_name>` folder

You should also be able to run `ng t` or `npm test` at this point, which will test the library using @angular/cli

Now you can begin adding new features/making bug fixes—please write tests around any of your changes. The code coverage for all of our modules lie somewhere between 50 and 80 percent code coverage. It would be nice to improve these numbers.

Once you are ready to view your changes in an actual application, `ng b` the library, `cd ./dist/<package_name>` and then run `npm pack` (this gets the compiled output ready for distribution)

Next, `cd` into your application of choosing, and run `npm i —save ../<package_name>/dist/<package_name>/<npm_packed_package_name>.tgz`

This will install the local version of your library into that application, and then you can simply invoke it within that applications source code, and `ng s` to view the results. If you do not `npm pack` the compiled lib output prior to installing it within an application, you will likely run into some misleading issues, I only say this because I have gone down that path before. 

Once you are happy with the changes, proceed to release

## Release

In order to release this package automatically, you must format the commit message properly so that when it is merged into master, it will semantically release the new changes based on commit msg type and previously tagged version (more info: https://www.notion.so/rentdynamics/Release-10-15-2018-270320233afb4d28838b5d4272512c06)

## Public Api

Don't forget to expose any new additions publically, ensure everything is accessible via the public_api.ts


[npm-icon]: https://nodei.co/npm/@rd/core.svg?downloads=true
[npm-icon-link]: https://npmjs.org/package/@rd/core
[circleci-badge]: https://circleci.com/gh/RentDynamics/ng-core.svg?style=shield
[circleci-link]: https://circleci.com/gh/rentdynamics/ng-core/tree/master
[codecov-image]: https://codecov.io/gh/RentDynamics/ng-core/branch/master/graph/badge.svg
[codecov-link]: https://codecov.io/gh/RentDynamics/ng-core
[nsp-image]: https://nodesecurity.io/orgs/rent-dynamics/projects/0b73ffc7-507b-4b70-ae71-035315f28a2e/badge
[nsp-link]: https://nodesecurity.io/orgs/rent-dynamics/projects/0b73ffc7-507b-4b70-ae71-035315f28a2e
[dependency-image]: https://david-dm.org/RentDynamics/ng-core/status.svg
[dependency-link]: https://david-dm.org/RentDynamics/ng-core
[dev-dependency-image]: https://david-dm.org/RentDynamics/ng-core/dev-status.svg
[dev-dependency-link]: https://david-dm.org/RentDynamics/ng-core?type=dev
[peer-dependency-image]: https://david-dm.org/RentDynamics/ng-core/peer-status.svg
[peer-dependency-link]: https://david-dm.org/RentDynamics/ng-core?type=peer
[public-true-image]: https://img.shields.io/badge/public-true-yellow.svg
[public-true-link]: https://img.shields.io/badge/public-true-yellow.svg
[private-true-image]: https://img.shields.io/badge/private-true-green.svg
[private-true-link]: https://img.shields.io/badge/private-true-green.svg
[npm-version-image]: https://img.shields.io/npm/v/@rd/core.svg
[npm-version-link]: https://www.npmjs.com/package/@rd/core
[npm-downloads-image]: https://img.shields.io/npm/dm/@rd/core.svg
[npm-downloads-link]: http://npm-stat.com/charts.html?package=@rd/core&from=2018-03-01
[npm-license-image]: https://img.shields.io/npm/l/@rd/core.svg
[npm-license-link]: LICENSE
[license-link]: http://opensource.org/licenses/MIT
