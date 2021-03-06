# `recetin`

This project is bootstrapped by [aurelia-cli](https://github.com/aurelia/cli).

For more information, go to https://aurelia.io/docs/cli/webpack

## Run dev app
> I personally use pnpm, you can always fallback to npm/yarn though

Run `pnpm start`, then open `http://localhost:8080`

You can change the standard webpack configurations from CLI easily with something like this: `pnpm start -- --open --port 8888`. However, it is better to change the respective pnpm scripts or `webpack.config.js` with these options, as per your need.

To enable Webpack Bundle Analyzer, do `pnpm run analyze` (production build).

To enable hot module reload, do `pnpm start -- --hmr`.

To change dev server port, do `pnpm start -- --port 8888`.

To change dev server host, do `pnpm start -- --host 127.0.0.1`

**PS:** You could mix all the flags as well, `pnpm start -- --host 127.0.0.1 --port 7070 --open --hmr`

For long time aurelia-cli user, you can still use `au run` with those arguments like `au run --env prod --open --hmr`. But `au run` now simply executes `pnpm start` command.

## Build for production

Run `pnpm run build`, or the old way `au build --env prod`.

## Unit tests

Run `au test` (or `au jest`).

To run in watch mode, `au test --watch` or `au jest --watch`.


## Build for Docker

This is as simple as running a command:

`yarn docker:build` or `pnpm run docker:build`

if you want to bring up an instance on your machine run:

`yarn docker:start` or `pnpm run docker:build`

to stop the previously started instance:

`yarn docker:stop` or `pnpm run docker:stop`
