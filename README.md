# @ailo/typescript-starter

Ailo Typescript library repo starter.

Features:

- TS strict preconfigured
- unit tests using Jest
- prettier, eslint, lint-staged, husky
- watch mode (run `yarn start` to run build compiler & unit tests in watch mode)
- two build targets: normal es2017, and esnext module

To start a new library (`@ailo/new-awesome-library`):

1. `git clone git@github.com:ailohq/typescript-starter.git new-awesome-library && cd new-awesome-library`
2. Create a `ailohq/new-awesome-library` repo on GH. (And add permissions to the `ailohq/core-team`.)
3. Add the repository to `#ailo-code-activity` Slack channel, so that the team can track commits pushed to remote by other people. The command is: `/github subscribe ailohq/typescript-starter`
4. `git remote rm origin && git remote add git@github.com:ailohq/new-awesome-library.git`
5. Search & replace everywhere in the repo `typescript-starter` to `new-awesome-library`.
6. Remove existing `src/**` files and add your own ones.
7. Remove `@ailo/ailorn` from package.json dependencies. Unless you actually need it. (It's added here just for a purpose of an example.)
8. Replace this description here with something meaningful. (For example, with description and a usage example of your library.)

**Note: There's no configuration here for CI (GoCD) yet.** Releasing is done manually, and linters/tests/build are being run during each `git push` / `yarn publish`.

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

**Note: Releasing is done manually (CI isn't configured yet).** Linters, tests, build and so on are run during each `git push` / `yarn release`.

```sh
yarn release # will automatically ask you about version bump, run tests and build, and push new version to git & npm
```
