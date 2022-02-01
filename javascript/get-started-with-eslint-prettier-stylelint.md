[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with ESLint, Prettier and Stylelint 🎨

## Installation

## ESLint 🔮

**What is ESLint 🔮**

[ESLint](https://www.npmjs.com/package/eslint) find and fix problems in your JavaScript code. It focuses on code errors
and best practices.

**Install ESLint 🔮 as dev dependencies**

```sh
# Base
npm install -D eslint

# If you develop React application
npm install -D eslint-config-airbnb

# If you develop NodeJS application
npm install -D eslint-config-airbnb-base

# Biased and opinionated config for Node
npm install -D eslint-config-node \
               eslint-plugin-node

# If you plan to use prettier
npm install -D eslint-config-prettier \
               eslint-plugin-prettier
```

Full installation for a React application
```sh
npm install -D eslint \
               eslint-config-airbnb \
               eslint-config-node \
               eslint-plugin-node \
               eslint-config-prettier \
               eslint-plugin-prettier
              
```

Full installation for a NodeJS application
```sh
npm install -D eslint \
               eslint-config-airbnb-base \
               eslint-config-node \
               eslint-plugin-node \
               eslint-config-prettier \
               eslint-plugin-prettier
```

TypeScript Support
```sh
npm install -D @typescript-eslint/eslint-plugin \
               @typescript-eslint/parser \
               eslint-config-airbnb-typescript
```

**Create `.eslintrc` file**

```json
{
    "extends": [
        "airbnb",      // Only for React
        "airbnb-base", // Only for NodeJS
        "node",
        "prettier"
    ],
    "plugins": ["node", "prettier"],
    "rules": {
        "arrow-body-style": "off",
        "indent": ["error", 4, {"SwitchCase": 1}],
        "import/prefer-default-export": "off",
        "prettier/prettier": ["error"]
    },
    "ignorePatterns": ["test/**/*", "jest.config.js","node_modules/**/*"]
}
```

TypeScript config
```json
{
    "extends": [
        "airbnb",      // Only for React
        "airbnb-base", // Only for NodeJS
        "airbnb-typescript/base",
        "node",
        "prettier",
        "plugin:@typescript-eslint/eslint-recommended",
        "plugin:@typescript-eslint/recommended"
    ],
    "parser": "@typescript-eslint/parser",
    "parserOptions": {
        "project": "tsconfig.json"
    },
    "plugins": ["node", "prettier", "@typescript-eslint"],
    "rules": {
        "arrow-body-style": "off",
        "indent": ["error", 4, {"SwitchCase": 1}],
        "import/prefer-default-export": "off",
        "prettier/prettier": ["error"]
    },
    "ignorePatterns": ["test/**/*", "jest.config.js","node_modules/**/*"]
}
```

## Prettier 🌟

**What is Prettier 🌟**

[Prettier](https://www.npmjs.com/package/prettier) is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.

**Install Prettier 🌟 as dev dependencies**

```sh
npm install -D prettier
```

**Create `.prettierrc` file**

```json
{
    "printWidth": 160,
    "tabWidth": 4,
    "useTabs": false,
    "semi": true,
    "singleQuote": true,
    "quoteProps": "as-needed",
    "jsxSingleQuote": false,
    "trailingComma": "none",
    "bracketSpacing": false,
    "bracketSameLine": true,
    "arrowParens": "always",
    "requirePragma": false,
    "insertPragma": false,
    "proseWrap": "preserve",
    "htmlWhitespaceSensitivity": "ignore",
    "endOfLine": "auto"
}
```

## StyleLint 🌟

**What is StyleLint 🌟**

[StyleLint](https://www.npmjs.com/package/stylelint) is a mighty, modern linter that helps you avoid errors and enforce conventions in your styles.

**Install StyleLint 🌟 as dev dependencies**

```sh
# Base and recommended config
npm install -D stylelint \
               stylelint-config-standard

# CSS preprocessor support (there is a less version too)
npm install -D postcss-scss

# CSS properties order support
npm install -D stylelint-order

# Recess config (recommended)
npm install -D stylelint-config-recess-order

# Idiomatic config (alternative, DO NOT INSTALL BOTH)
npm install -D stylelint-config-idiomatic-order
```

Full installation
```sh
npm install -D stylelint \
               stylelint-config-standard \
               postcss-scss \
               stylelint-order \
               stylelint-config-recess-order
```

**Create `.stylelintrc` file**

```json
{
    "extends": ["stylelint-config-standard", "stylelint-config-recess-order"],
    "plugins": ["stylelint-order"],
    "customSyntax": "postcss-scss",
    "rules": {
        "indentation": 4
    }
}

```

## It works !

*Don't forget to give a* ⭐️ *if this markdown helped you !*
