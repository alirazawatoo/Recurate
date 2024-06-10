# Recurate GitHub Repository Service

A Node.js/TypeScript service that calls the GitHub API and exposes repository information through versioned routes described by `docs/api-spec.yaml`.

```bash
cp .env.example .env
npm install
npm run dev
```

Set `GITHUB_PERSONAL_ACCESS_TOKEN`, `PORT`, and `API_VERSION`; use minimum token scope and never commit it. `RepoController.ts` and `routes/index.ts` contain the request flow, with router tests under `tests`. Rate limits, pagination, permission errors, and caching require further production work.
