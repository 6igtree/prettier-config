# @6igtree/prettier-config

My shared [Prettier](https://prettier.io/) config. Only the options that differ from Prettier's defaults are set:

```json
{
  "semi": false,
  "singleQuote": true,
  "useTabs": true,
  "trailingComma": "es5"
}
```

## Install

```sh
npm install --save-dev prettier github:6igtree/prettier-config
```

## Usage

Add this to your `package.json`:

```json
{
  "prettier": "@6igtree/prettier-config"
}
```

To override an option, use a `prettier.config.mjs` instead, and remove the `"prettier"` key from `package.json` (it takes precedence):

```js
import config from '@6igtree/prettier-config' with { type: 'json' }

export default {
	...config,
	printWidth: 100,
}
```
