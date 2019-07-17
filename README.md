# React Component Library Template

A template repository for creating a React component library for use in React applications. This builds
es, esm, cjs, and umd builds of your library.

This library can be used inside workspaces as well so you can build a library and then
import components just as if it was published to npm (or github packages) and installed that way.

## Usage

Create a new repository from this template, or copy the files from this template and then edit
the package.json to change the name and product name. Add any other dependencies, etc... you require.

Run `yarn build` to build all code into dist. You should now be able to use commonjs or javascript module imports to import code directly.

## Publishing

By default, the package.json is configured for github package repository. To use npm, remove the `publishConfig` section in the package.json:

```
  "publishConfig": {
    "registry": "https://npm.pkg.github.com/"
  },
```

To publish, cd in dist after running a build then run publish.

```
yarn build
cd ./dist
yarn publish
```
