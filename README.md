[![Piral Logo](https://github.com/smapiot/piral/raw/develop/docs/assets/logo.png)](https://piral.io)

# [Piral Sample](https://piral.io) &middot; [![GitHub License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/smapiot/piral/blob/main/LICENSE) [![Gitter Chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/piral-io/community)

> Piral Webpack Sample

:zap: These examples show how to use Piral with Webpack, specifically the `piral-cli-webpack` plugin.

We have two folders.

## `sample-pilet`

Shows how a standard pilet is debugged and build using Webpack.

After scaffolding we installed `piral-cli-webpack`:

```sh
npm i piral-cli-webpack --save-dev
```

We've updated the `start` and `build` npm tasks to use `pilet debug-wp` and `pilet build-wp` respectively.

Besides the change of the two commands we also show here how to publish a pilet in one command:

```sh
npm run publish
```

Which just uses the following commands:

```sh
 # cleanup first
rm -rf dist
# also remove old tgz files
rm -f *.tgz
# build it (using webpack!)
npm run build
# pack it using the Piral CLI
pilet pack
# publish the last packed file
pilet publish --url https://feed.piral.cloud/api/v1/pilet/empty --api-key is-invalid-anyway
```

## `sample-piral-instance`

Shows how a Piral instance is debugged and build using Webpack.

After scaffolding we installed `piral-cli-webpack`. Since the Piral instance also used Sass for the stylesheet we had to install `node-sass`, too:

```sh
npm i piral-cli-webpack node-sass --save-dev
```

We've updated the `start` and `build` npm tasks to use `piral debug-wp` and `piral build-wp` respectively.

## License

Piral and this sample code is released using the MIT license. For more information see the [license file](./LICENSE).
