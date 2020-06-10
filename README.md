# TypeScript template

Template repository for TypeScript projects with Babel.

## Development workflow

To get started with the project, run `yarn` in the root directory to install the required dependencies:

```sh
yarn
```

When making changes, make sure your code passes TypeScript and ESLint. Run the following to verify:

```sh
yarn lint
yarn typescript
```

To fix formatting errors, run the following:

```sh
yarn lint --fix
```

While developing, you can run the typescript type-checker in watch mode:

```sh
yarn typescript --watch
```

Remember to add tests for your change if possible. Run the unit tests by:

```sh
yarn test
```

While developing, you can run the tests in watch mode:

```sh
yarn test --watch
```

### Commit message convention

We follow the [conventional commits specification](https://www.conventionalcommits.org/en) for our commit messages:

- `fix`: bug fixes, e.g. fix crash due to deprecated method.
- `feat`: new features, e.g. add new method to the module.
- `refactor`: code refactor, e.g. migrate from class components to hooks.
- `docs`: changes into documentation, e.g. add usage example for the module..
- `test`: adding or updating tests, eg add integration tests using detox.
- `chore`: tooling changes, e.g. change CI config.

Our pre-commit hooks verify that your commit message matches this format when committing.

### Linting and tests

[ESLint](https://eslint.org/), [Prettier](https://prettier.io/), [TypeScript](https://www.typescriptlang.org/)

We use [TypeScript](https://www.typescriptlang.org/) for type checking, [ESLint](https://eslint.org/) with [Prettier](https://prettier.io/) for linting and formatting the code, and [Jest](https://jestjs.io/) for testing.

Our pre-commit hooks verify that the linter and tests pass when committing.

### Scripts

The `package.json` file contains various scripts for common tasks:

- `yarn typescript`: type-check files with TypeScript.
- `yarn lint`: lint files with ESLint.
- `yarn test`: run unit tests with Jest.
- `yarn releases`: publish the library to npm.
