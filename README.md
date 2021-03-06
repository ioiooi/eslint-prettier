# ESLint and Prettier

## Why ESLint and Prettier?

[Linters have two categories of rules: Formatting and Code-quality rules](https://prettier.io/docs/en/comparison.html)  
Prettier formatting looks better than ESLint.

## Installation

[Prettier integration with ESLint](https://prettier.io/docs/en/eslint.html)  
`npm install --save-dev prettier eslint eslint-plugin-prettier eslint-config-prettier`

1.  `eslint` and `prettier`
2.  `eslint-plugin-prettier` ([link](https://github.com/prettier/eslint-plugin-prettier))  
    ESLint will run Prettier for you and will report formatting issues between your code and Prettiers configuration as ESLint issues.
3.  `eslint-config-prettier` ([link](https://github.com/prettier/eslint-config-prettier))  
    Turns off all ESLint formatting rules that are unnecessary or might conflict with Prettier.
4.  _Optional: `eslint-plugin-react`  
    React specific linting rules for ESLint._

## eslintrc config

import/export, async/await and support for other newer features

```json
"parserOptions": {
  "sourceType": "module",
  "ecmaVersion": 2018
}
```

React, ESLint defaults, [`eslint-plugin-prettier` and `eslint-config-prettier`](https://prettier.io/docs/en/eslint.html#why-not-both)

```json
"extends": [
  "eslint:recommended",
  "plugin:prettier/recommended"
]
```

[Customize Prettier options.](https://github.com/prettier/eslint-plugin-prettier#options)

```json
"prettier/prettier": ["error", { "singleQuote": true }]
```
