## Create a new Skeleton / SvelteKit Project

[Skeleton](https://www.skeleton.dev/) allows you to create adaptive and accessible interfaces for web apps of any shape or size.

Use the [Skeleton CLI](https://www.skeleton.dev/docs/get-started) for creating new Skeleton projects (rather than `pnpm create svelte@latest`). This will automatically scaffold a new SvelteKit application, install [Tailwind CSS](https://tailwindcss.com/), configure Skeleton, and more:

```bash
pnpm create skeleton-app@latest
```

```
Welcome to Skeleton 💀! A UI toolkit for Svelte + Tailwind

Problems? Open an issue on https://github.com/skeletonlabs/skeleton/issues.
│
◇  Which Skeleton app template?
│  AppShell starter
│
◇  Select a theme (top most selection will be default):
│  Skeleton
│
◇  Enter a name for your custom theme:
│  my-custom-theme
│
◇  What other packages would you like to install:
│  Add Tailwind forms, Add Tailwind typography
│
◇  Add type checking with TypeScript?
│  Yes, using TypeScript syntax
│
◇  What would you like setup in your project:
│  Add ESLint, Add Prettier, Add Vitest, Add Svelte Inspector
│
◇  Done installing
```

The CLI will automatically install Skeleton and the Skeleton Tailwind plugin, along with the [`@types/node`](https://www.npmjs.com/package/@types/node) standard Node type definitions, which reduce nuisance linting messages in Typescript projects.

### Install dependencies

```
cd my-skeleton-project
pnpm install
```

## Add a Theme

If the Skeleton CLI worked properly, the following items will have been completed automatically. But a quick verification ensures that everything is working correctly.

1.  Register your preferred theme (or themes) in `tailwind.config.ts`:

```ts
plugins: [
	skeleton({
		themes: { preset: ['skeleton'] }
	})
];
```

2.  Open `/src/app.html` and set the active theme using the `data-theme` attribute:

```html
<body data-theme="skeleton"></body>
```

## Start the Dev Server

```bash
pnpm dev
```

## Building for Production

To create a production version of your app, run:

```bash
pnpm build
```

You can preview the production build with `pnpm preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
