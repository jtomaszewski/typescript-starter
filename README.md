# @ailo/typescript-starter

Ailo Typescript library repo starter. Fork this to begin a new TS library based it on this starter.

Features:

- TS strict preconfigured
- unit tests using Jest
- prettier, eslint, lint-staged, husky
- watch mode (run `yarn start` to run build compiler & unit tests in watch mode)
- two build targets: normal es2017, and esnext module

**Note: There's no configuration here for CI (GoCD) yet.** Releasing is done manually.

## Development

```
yarn
yarn start
```

## Testing

```
yarn lint # prettier and eslint
yarn test # unit tests
yarn test:watch # unit tests in watch mode
```

## Releasing

```
git push
yarn publish # will automatically ask you about version bump, run tests and build, and push new version to git & npm
```
