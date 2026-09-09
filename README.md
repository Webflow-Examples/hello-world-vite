# Vite + React + TypeScript + Webflow Cloud

Example [Vite](https://vite.dev) + React + TypeScript app with a [Hono](https://hono.dev) worker on Cloudflare, configured for [Webflow Cloud](https://webflow.com/cloud).

[![Deploy to Webflow](https://webflow.com/img/deploy-dark.svg)](https://webflow.com/dashboard/cloud/deploy?repo=https://github.com/Webflow-Examples/hello-world-vite)

## Project structure

```text
.
├── index.html
├── LICENSE
├── package.json
├── package-lock.json
├── public
│   ├── hono.svg
│   ├── vite.svg
│   └── webflow.svg
├── src
│   ├── App.tsx
│   ├── globals.d.ts
│   ├── main.tsx
│   ├── style.css
│   └── worker.ts
├── tsconfig.json
├── vite.config.ts
├── webflow.json
├── worker-configuration.d.ts
└── wrangler.json
```

`src/main.tsx` mounts the React app in `src/App.tsx`. `src/worker.ts` is the Hono
worker that serves the `/api/hello` endpoint and the built static assets.

## Commands

| Command              | Action                                                                              |
| -------------------- | ----------------------------------------------------------------------------------- |
| `npm install`        | Install dependencies.                                                               |
| `npm run dev`        | Start the Vite dev server (default [http://localhost:5173](http://localhost:5173)). |
| `npm run build`      | Production-build the app to `dist/`.                                                |
| `npm run preview`    | Serve the production build locally (default [http://localhost:4173](http://localhost:4173)). |
| `npm run deploy`     | Deploy to Webflow Cloud with the Webflow CLI.                                       |
| `npm run cf-typegen` | Regenerate `worker-configuration.d.ts` from `wrangler.json`.                        |

## Learn more

- [Vite documentation](https://vite.dev)
- [Hono documentation](https://hono.dev)
- [Webflow Cloud](https://webflow.com/cloud)
