# @ridecell/eslint-config-react

ESLint configuration for Ridecell React apps

## Installation

First, install this package, ESLint and the necessary plugins.

```bash
npm install --save-dev @ridecell/eslint-config-react babel-eslint@7.2.3 eslint@4.6.1
eslint-config-airbnb@15.1.0 eslint-plugin-import@2.7.0 eslint-plugin-jsx-a11y@5.1.1 eslint-plugin-react@7.1.0
```

Then create a file named .eslintrc with following contents in the root folder of your project:

```json
{
  "extends": "@ridecell/eslint-config-react"
}
```

That's it! You can override the settings by editing the .eslintrc file.

## Development

To test changes to the lint rules against code, use `npm-link` in a project. [Helpful guide](http://justjs.com/posts/npm-link-developing-your-own-npm-modules-without-tears)
