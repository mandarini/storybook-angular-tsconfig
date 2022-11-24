# Contents

Angular application, configured with Storybook. Changed Storybook configuration file (`main.js`) to `main.ts`, as described [here](https://storybook.js.org/docs/react/configure/overview#configure-your-project-with-typescript).

## Steps I followed

1. `ng new my-app`
2. `npx sb init`
3. Steps decsribed [here](https://storybook.js.org/docs/angular/configure/overview#configure-your-project-with-typescript), renamed `main.js` to `main.ts`, adjusted contents, created `.babelrc` file.

## Storybook does not work

```
yarn storybook
```

and

```
yarn build-storybook
```

and

```
ng run my-app:storybook
```

and

```
ng build my-app:build-storybook
```

fail with this error:

```
ERR! Error: Debug Failure. False expression: Non-string value passed to `ts.resolveTypeReferenceDirective`, likely by a wrapping package working with an outdated `resolveTypeReferenceDirectives` signature. This is probably not a problem in TS itself.
ERR!     at Object.resolveTypeReferenceDirective (/Users/katerina/Projects/nrwl/SB-NG/my-app/node_modules/typescript/lib/typescript.js:43193:18)
ERR!     at /Users/katerina/node_modules/ts-node/src/index.ts:623:55
ERR!     at Array.map (<anonymous>)
ERR!     at Object.resolveTypeReferenceDirectives (/Users/katerina/node_modules/ts-node/src/index.ts:622:33)
ERR!     at actualResolveTypeReferenceDirectiveNamesWorker (/Users/katerina/Projects/nrwl/SB-NG/my-app/node_modules/typescript/lib/typescript.js:118257:163)
ERR!     at resolveTypeReferenceDirectiveNamesWorker (/Users/katerina/Projects/nrwl/SB-NG/my-app/node_modules/typescript/lib/typescript.js:118557:26)
ERR!     at processTypeReferenceDirectives (/Users/katerina/Projects/nrwl/SB-NG/my-app/node_modules/typescript/lib/typescript.js:120054:31)
ERR!     at findSourceFileWorker (/Users/katerina/Projects/nrwl/SB-NG/my-app/node_modules/typescript/lib/typescript.js:119939:21)
ERR!     at findSourceFile (/Users/katerina/Projects/nrwl/SB-NG/my-app/node_modules/typescript/lib/typescript.js:119791:26)
ERR!     at processImportedModules (/Users/katerina/Projects/nrwl/SB-NG/my-app/node_modules/typescript/lib/typescript.js:120200:25)
```
