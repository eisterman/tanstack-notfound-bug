# Bug Report
Repo used to showcase a strange bug where a specific route structure and a throw notFound() crash a layout with hydratation error.

## How to Launch
```
pnpm install
pnpm dev
```

## Instruction to reproduce the bug
1. Launch the app
2. Navigate manually to a Post page that doesn't exist like `/posts/i-do-not-exist`
3. The error that appear is caused by the `Route.useLoaderData()` that return undefined during the layout render.
