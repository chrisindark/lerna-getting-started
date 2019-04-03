## Getting started.

```
npm i lerna -g
```

```
lerna init
```

```
lerna bootstrap
```

```
.
├── README.md
├── lerna.json
├── package.json
└── packages
    ├── alpha
    │   ├── index.js
    │   ├── node_modules
    │   └── package.json
    ├── beta
    │   ├── index.js
    │   ├── node_modules
    │   └── package.json
    └── usage
        ├── index.js
        ├── node_modules
        │   ├── alpha
        │   │   ├── index.js
        │   │   └── package.json
        │   └── beta
        │       ├── index.js
        │       └── package.json
        └── package.json
```

When we run `node ./packages/usage/index.js` we get our expected output:
```
alpha beta
```
