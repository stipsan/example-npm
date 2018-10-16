# npm GitHub Action Example

An example workflow, using [the GitHub Action for npm](https://github.com/actions/npm) to build, test, and publish an npm module, [`@scrabblescore/scrabblescore`](https://www.npmjs.com/package/@scrabblescore/scrabblescore).

## Workflow

The [example workflow](.github/main.workflow) will trigger on every push to this repo.

For pushes to a _feature_ branch, the workflow will:

1. Run `npm install`, to install the module's prerequisites
1. Run `npm test`, to run the module's unit tests

For pushes to the _default_ branch (`master`), in addition to the above Actions, the workflow will:

1. Run `npm publish`, to release the module to the world

## License

This repository is [licensed under CC0-1.0](LICENSE), which waives all copyright restrictions.
