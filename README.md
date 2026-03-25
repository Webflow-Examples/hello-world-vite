# Vite + TypeScript + Webflow Cloud

Example Vite + TypeScript app with a Hono worker on Cloudflare, configured for [Webflow Cloud](https://webflow.com/cloud).

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
│   ├── api.ts
│   ├── counter.ts
│   ├── globals.d.ts
│   ├── main.ts
│   ├── style.css
│   └── worker.ts
├── tsconfig.json
├── vite.config.ts
├── webflow.json
├── worker-configuration.d.ts
└── wrangler.json
```

## Commands

| Command | Action |
| --- | --- |
| `npm install` | Install dependencies. |
| `npm run dev` | Generate Wrangler types, then start the Vite dev server (default [http://localhost:5173](http://localhost:5173)). |
| `npm run build` | Generate Wrangler types, run `tsc`, then production-build the app to `dist/`. |
| `npm run preview` | Generate Wrangler types, then serve the production build locally (default [http://localhost:4173](http://localhost:4173)). |

## Learn more

- [Vite documentation](https://vite.dev)
- [Webflow Cloud](https://webflow.com/cloud)
