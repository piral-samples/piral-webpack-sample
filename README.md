# Piral Webpack Sample

These examples show how to use Piral with Webpack, specifically the `piral-cli-webpack` plugin.

We have two folders.

## `sample-pilet`

Shows how a standard pilet is debugged and build using Webpack.

After scaffolding we installed `piral-cli-webpack`:

```sh
npm i piral-cli-webpack --save-dev
```

We've updated the `start` and `build` npm tasks to use `pilet debug-wp` and `pilet build-wp` respectively.

## `sample-piral-instance`

Shows how a Piral instance is debugged and build using Webpack.

After scaffolding we installed `piral-cli-webpack`. Since the Piral instance also used Sass for the stylesheet we had to install `node-sass`, too:

```sh
npm i piral-cli-webpack node-sass --save-dev
```

We've updated the `start` and `build` npm tasks to use `piral debug-wp` and `piral build-wp` respectively.