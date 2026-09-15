# SvelteKit + Tailwind Template

A minimal SvelteKit starter template with TypeScript, Tailwind CSS, and Prettier configured for automatic Tailwind class sorting.

## What's included

* [SvelteKit](https://svelte.dev/)
* [Svelte 5](https://svelte.dev/)
* TypeScript
* [Tailwind CSS 4](https://tailwindcss.com/)
* [Vite](https://vite.dev/)
* [Prettier](https://prettier.io/)
* `prettier-plugin-svelte`
* `prettier-plugin-tailwindcss`
* [pnpm](https://pnpm.io/)
* VS Code formatting on save
* Tailwind CSS IntelliSense

## Getting started

### Use this template

Click **Use this template** on GitHub to create a new repository from this template.

Clone your new repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_PROJECT.git
cd YOUR_PROJECT
```

### Install dependencies

This project uses pnpm.

```bash
pnpm install
```

### Start the development server

```bash
pnpm dev
```

The development server will be available at:

```text
http://localhost:5173
```

## Available commands

| Command        | Description                       |
| -------------- | --------------------------------- |
| `pnpm dev`     | Start the development server      |
| `pnpm build`   | Create a production build         |
| `pnpm preview` | Preview the production build      |
| `pnpm check`   | Run Svelte and TypeScript checks  |
| `pnpm format`  | Format the project with Prettier  |
| `pnpm lint`    | Check formatting and code quality |

## Tailwind CSS

This template uses Tailwind CSS 4.

Tailwind classes are automatically sorted by Prettier using `prettier-plugin-tailwindcss`.

For example:

```svelte
<div class="text-white px-4 flex bg-blue-500 items-center">
  Hello
</div>
```

is formatted to:

```svelte
<div class="flex items-center bg-blue-500 px-4 text-white">
  Hello
</div>
```

You don't need to manually maintain the order of Tailwind utility classes.

## Prettier

Prettier is configured with:

* `prettier-plugin-svelte` for Svelte files
* `prettier-plugin-tailwindcss` for automatic Tailwind class sorting

The template is configured to use Prettier automatically when saving Svelte files in VS Code.

## VS Code

The repository includes VS Code settings in:

```text
.vscode/settings.json
```

These settings configure Prettier as the default formatter for Svelte files and enable formatting on save.

For the best development experience, install:

* **Prettier - Code formatter**
* **Tailwind CSS IntelliSense**

## Project structure

```text
.
├── src/
│   ├── lib/
│   │   ├── assets/
│   │   └── index.ts
│   ├── routes/
│   │   ├── +layout.svelte
│   │   └── +page.svelte
│   ├── app.css
│   ├── app.d.ts
│   └── app.html
├── static/
│   └── robots.txt
├── .gitignore
├── .prettierrc
├── package.json
├── pnpm-lock.yaml
├── pnpm-workspace.yaml
├── tsconfig.json
└── vite.config.ts
```

## Building for production

Create a production build:

```bash
pnpm build
```

Preview the production build locally:

```bash
pnpm preview
```

The project currently uses SvelteKit's adapter-auto, so the appropriate deployment adapter can be added depending on your hosting platform.

## Customizing the template

After creating a repository from this template, update:

* `package.json` — project name and metadata
* `README.md` — project-specific documentation
* `src/` — application code
* `static/` — static assets
* SvelteKit adapter — depending on your deployment platform

## License

Add a license to this repository if you intend to distribute the template publicly.
