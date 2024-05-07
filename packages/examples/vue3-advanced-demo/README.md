# Vue3 Module Federation Vitest Bug Reproduction Steps

This example demos consumption of federated modules from a vite bundle. `layout` app depends on components exposed by `home`, `common-lib` and `css-modules` app.

## Reproduction Steps

1. Clone [adarshdeep-ld/vite-plugin-federation](https://github.com/adarshdeep-ld/vite-plugin-federation) if you haven't already.
2. At the repository root, install dependencies (`pnpm install`) and build (`pnpm build`).
3. Go to this example folder: `cd packages\examples\vue3-advanced-demo`
4. Run `pnpm install`, `pnpm build` and `pnpm serve` . This will build and serve all services
5. Open a new terminal window and run`cd team-red`
6. Run `npm run test:unit`

Go To: [localhost:5000](http://localhost:5000/)

`CTRL + C` can only stop the host server. You can run `pnpm stop` to stop all services.
