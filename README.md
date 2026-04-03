# Astro Starter Kit: Minimal

```sh
npm create astro@latest -- --template minimal
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## CI/CD & Deployment

### GitHub Actions CI

A CI workflow runs automatically on every push and pull request to `main` and `dev`:

- **Install**: `npm ci`
- **Build**: `npm run build` — PR merges are blocked if the build fails
- **Lint**: `npm run lint` (skipped if not configured)

Workflow file: `.github/workflows/ci.yml`

### Vercel Deployment

The project is connected to Vercel for automatic deployments:

- Pushes to `main` trigger a **production deployment** (auto-deploys within ~2 minutes)
- Pushes to `dev` trigger a **preview deployment**

### Branch Strategy

| Branch | Purpose |
| :----- | :------ |
| `main` | Production — deploys to live site |
| `dev`  | Integration — feature branches merge here first |

All code changes go through `dev` first, then are merged to `main` via PR after review.

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
