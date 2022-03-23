# Image Transform Service

[![TypeScript version][ts-badge]][typescript-4-6]
[![Node.js version][nodejs-badge]][nodejs]
[![APLv2][license-badge]][license]
[![Build Status - GitHub Actions][gha-badge]][gha-ci]

🌄 An example project for an Image Transforming Service.

This is a pure [ESM][esm] project intended to be used with the latest Active LTS release of [Node.js][nodejs].

## Getting Started

1. Copy `.env.template` as `.env` and fill the required variables.
2. run `yarn build`
3. run `yarn start`

## Available Scripts

- `start` - start the server.
- `dev` - start and restart the server on file changes.
- `clean` - remove coverage data, Jest cache and transpiled files.
- `prebuild` - lint source files and tests before building.
- `build` - transpile TypeScript to ES6.
- `build:watch` - interactive watch mode to automatically transpile source files.
- `lint` - lint source files and tests.
- `test` - run tests.
- `test:watch` - interactive watch mode to automatically re-run tests.

## Docker

The project can be started using `docker-compose`

```
docker-compose up
```

## Usage

Assuming the server is started with `PORT=3000`. The following REST APIs are exposed:

- **GET** `http://localhost:3000/api/v1/images?source=image-url&height=1024&width=1024&fit=cover&quality=90`

  Transform the image of `source` followed with any of the options `width`, `height`, `fit` and `quality`

## Notes

This project is started from [node-typescript-boilerplate][node-typescript-boilerplate] template.

## License

Licensed under the APLv2. See the [LICENSE][license] file for details.

[ts-badge]: https://img.shields.io/badge/TypeScript-4.6-blue.svg
[nodejs-badge]: https://img.shields.io/badge/Node.js->=%2016.13-blue.svg
[nodejs]: https://nodejs.org/dist/latest-v14.x/docs/api/
[esm]: https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c
[gha-badge]: https://github.com/jsynowiec/node-typescript-boilerplate/actions/workflows/nodejs.yml/badge.svg
[gha-ci]: https://github.com/jsynowiec/node-typescript-boilerplate/actions/workflows/nodejs.yml
[typescript-4-6]: https://devblogs.microsoft.com/typescript/announcing-typescript-4-6/
[license-badge]: https://img.shields.io/badge/license-APLv2-blue.svg
[license]: ./LICENSE
[node-typescript-boilerplate]: https://github.com/jsynowiec/node-typescript-boilerplate
