# eslint-config-jonyamo-base

A basic [ESLint](https://eslint.org) and [Prettier](https://prettier.io) configuration.

## Installation

Install ESLint and Prettier:

```shell
$ yarn add eslint prettier --dev
```

Install this package:

```shell
$ yarn add eslint-config-jonyamo-base --dev
```

## Configuration

Add an `extends` section to your `.eslintrc` (or [equivalent](https://eslint.org/docs/user-guide/configuring#configuration-file-formats)) and specify `jonyamo-base` as an extended configuration. Rules can be adjusted by overriding them in the `rules` section. E.g.:

```js
// .eslintrc.js

module.exports = {
    extends: ['jonyamo-base'],
    rules: {
        'unicorn/prevent-abbreviations': 'off',
    },
};
```
