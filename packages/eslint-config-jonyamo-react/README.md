# eslint-config-jonyamo-react

[React](https://reactjs.org/) specific [ESLint](https://eslint.org) and [Prettier](https://prettier.io) configuration.

## Installation

Install ESLint and Prettier:

```shell
$ yarn add eslint prettier --dev
```

Install this package:

```shell
$ yarn add eslint-config-jonyamo-react --dev
```

## Configuration

Add an `extends` section to your `.eslintrc` (or [equivalent](https://eslint.org/docs/user-guide/configuring#configuration-file-formats)) and specify `jonyamo-react` as an extended configuration. Rules can be adjusted by overriding them in the `rules` section. E.g.:

```js
// .eslintrc.js

module.exports = {
    extends: ['jonyamo-react'],
    rules: {
        'react/jsx-curly-newline': 'off',
    },
};
```
