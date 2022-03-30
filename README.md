# Project No. 2 with a demonstration of the problem

In this project, the php-storm-issue-1 package is included from a neighboring repository in the account.
There are 2 aliases in the `vue.config.js` and `tsconfig.json` file that refer to `/node_modules/php-storm-issue-1/src/components`

The App.vue file demonstrates the issue:
* Importing the `MyComponent1` component using the `@components` alias (path: `/node_modules/php-storm-issue-1/src/components/MyComponent.vue`) shows an error
* Importing the `MyComponent2` component using the `@components` alias (path: `/src/components/MyComponent.vue`) **DOES NOT** show an error
* Importing the `MyComponent1` component using the `#components` alias (path: `/node_modules/php-storm-issue-1/src/components/MyComponent.vue`) **DOES NOT** show an error

However, the code itself works. This can be verified by running a test server:
```
npm run serve
```

Package installation command:
```
npm i git+https://github.com/PurpleTape/PhpStormIssueRef.git#0.1.0
```
