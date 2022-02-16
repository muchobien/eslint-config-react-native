# eslint-config-react-native

## Use

### Configure tsconfig.json

```json
{
  "extends": "@muchobien/eslint-config-react-native/tsconfig.base",
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@app": ["./src"],
      "@app/*": ["./src/*"]
    }
  },
  "exclude": [
    "node_modules",
    "babel.config.js",
    "metro.config.js",
    "jest.config.js",
    "commitlint.config.js"
  ]
}
```

### Configure .eslintrc.js

```js
module.exports = {
  root: true,
  extends: '@muchobien/eslint-config-react-native',
};
```