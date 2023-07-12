# eslint-config-strict - WIP
A strict TypeScript ESM based ESLint config for backends aimed at avoiding potential bugs, removing redundancy, improving code clarity, and of course, enforcing consistency. In addition to the aforementioned traits this config also aims to enforce the use of newer, more recommended functions and language features.

## Included Rules
The eslint config extends the following configs:

```
eslint:recommended
eslint-config-prettier
```

and the following plugins:
```
@typescript-eslint/recommended
@typescript-eslint/recommended-requiring-type-checking
unicorn/recommended
```

The following, additional rules are also enabled:
#### [ESLint](https://eslint.org/docs/latest/rules/)
```
"constructor-super": "error",
"for-direction": "error",
"no-await-in-loop": "error",
"no-constant-binary-expression": "error",
"no-duplicate-imports": "error",
"no-new-native-nonconstructor": "error",
"no-promise-executor-return": "error",
"no-self-compare": "error",
"no-template-curly-in-string": "error",
"no-unmodified-loop-condition": "error",
"no-unreachable-loop": "error",
"no-unused-private-class-members": "error",
"require-atomic-updates": "error",
"no-use-before-define": "error",
"camelcase": "error",
```

#### [TypeScript ESLint](https://typescript-eslint.io/rules/)
```
"@typescript-eslint/adjacent-overload-signatures": "error",
"@typescript-eslint/array-type": ["error", { "default": "generic" }],
"@typescript-eslint/consistent-type-exports": "error",
"@typescript-eslint/consistent-type-imports": "error",
"@typescript-eslint/explicit-function-return-type": "error",
"@typescript-eslint/explicit-module-boundary-types": "error",
"@typescript-eslint/no-duplicate-type-constituents": "error",
"@typescript-eslint/no-confusing-void-expression": "error",
"@typescript-eslint/no-import-type-side-effects": "error",
"@typescript-eslint/no-require-imports": "error",
"@typescript-eslint/no-unused-vars": "error",
"@typescript-eslint/no-useless-empty-export": "error",
"@typescript-eslint/prefer-enum-initializers": "error",
"@typescript-eslint/prefer-readonly": "error",
"no-return-await": "off",
"@typescript-eslint/return-await": "error",
```

#### [Unicorn](https://github.com/sindresorhus/eslint-plugin-unicorn#rules)
```
"unicorn/custom-error-definition": "error",
"unicorn/no-array-reduce": "off",
"unicorn/no-null": "off"
```

## Install
Run the following command inside of a node project:

`npm install @ricardovaldovinosorg/eslint-config-strict`

## Usage
After installing the npm package create the following .eslintrc file in your project
```
{ "extends": ["@ricardovaldovinosorg/eslint-config-strict"] }
```
