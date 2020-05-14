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

### Create React App

For apps built with [`create-react-app`](https://create-react-app.dev), in order to extend the included base config follow [these instructions](https://create-react-app.dev/docs/setting-up-your-editor#experimental-extending-the-eslint-config), which basically state:

1. In `.env` set:

```
EXTEND_ESLINT=true
```

2. In `package.json`:

```json
{
    "eslintConfig": {
        "extends": ["react-app", "jonyamo-react"]
    }
}
```
