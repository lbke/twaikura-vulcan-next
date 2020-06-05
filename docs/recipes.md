## Magic imports

- Use the `paths` property of tsconfig.common.json.
- Add an alias in Next's Webpack config
- Add an alias in Jest moduleNameMapper config

[Relevant documentation](https://www.typescriptlang.org/docs/handbook/module-resolution.html)

### Why 2-steps?

Using TypeScript `paths` will only tell TypeScript where to find the code. However, it won't replace your import path at build time.

So, you also need Webpack to actually replace `~/components/myComponent` to `../../../components/myComponent`.

## Debugging Cypress build

See [Cypress Webpack Preprocessor doc](https://github.com/cypress-io/cypress-webpack-preprocessor), it describes a few environment variables useful to debug Cypress build.

## Mock next packages
