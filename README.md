# @ailo/typescript-starter

Ailo Typescript library repo starter.

Features:

- TS strict preconfigured
- unit tests using Jest
- prettier, eslint, lint-staged, husky
- watch mode (run `yarn start` to run build compiler & unit tests in watch mode)
- two build targets: normal es2017, and esnext module

To start a new library (`@ailo/new-awesome-library`):

1. `git clone @ailo/typescript-stater ailo-new-awesome-library && cd ailo-new-awesome-library`
2. Create a `ailohq/ailo-new-awesome-library` repo on GH.
3. `git remote rm origin && git remote add git@github.com:ailohq/ailo-new-awesome-library.git`
4. Search & replace everywhere in the repo `typescript-starter` to `new-awesome-library`.
5. Remove existing `src/**` files and add your own ones.
6. Remove `@ailo/ailorn` from package.json dependencies. Unless you actually need it. (It's added here just for a purpose of an example.)
7. Replace this description here with something meaningful. (For example, with description and a usage example of your library.)

**Note: There's no configuration here for CI (GoCD) yet.** Releasing is done manually, and linters/tests/build are on each `git push` / `yarn publish`. (Which should be fine with small, rarely updated libraries I guess.)

## Development

```sh
yarn
yarn start
```

## Testing

```sh
yarn lint # prettier and eslint
yarn test # unit tests
yarn test:watch # unit tests in watch mode
```

## Releasing

```sh
yarn release # will automatically ask you about version bump, run tests and build, and push new version to git & npm
```
