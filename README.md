# Next

**Reactivity > Inspecting State**

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
pnpm run dev

# or start the server and open the app in a new browser tab
pnpm run dev -- --open
```

## Building

To create a production version of your app:

```bash
pnpm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.

## Notes

- Effects do not run during server side rendering
- You cannot export a $state declaration from a module if the declaration is reassigned (rather than just mutated), because the importers would have no way to know about it.
