# @ridecell/eslint-config-react

ESLint configuration for Ridecell React apps

## Installation

Run the following command in your project root directory:

```bash
yarn add --dev @ridecell/eslint-config-react
```

Then you need to create 3 files:

 1. `.eslintrc` with the following content:

```json
{
  "parser": "babel-eslint",
  "extends": "@ridecell/eslint-config-react"
}
```

 2. `.prettierrc.js` with the following content:

```javascript
module.exports = require('@ridecell/eslint-config-react/.prettierrc')
```

 3. `.prettierignore` with the following content:

```
*.json
node_modules
dist
```

That's it! You can always override those setting.

## Prettier

You can add the following 2 commands to your `package.json` scripts

 1. `"prettier-changed": "pretty-quick",` - prettifies only the files that were changed
 2. `"prettier-all": "prettier --write \"**/*.{js,jsx}\""` - prettifies all the files


## Development

To test changes to the lint rules against code, use `npm-link` in a project. [Helpful guide](http://justjs.com/posts/npm-link-developing-your-own-npm-modules-without-tears)
