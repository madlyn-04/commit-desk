# CommitDesk

CommitDesk turns meeting notes and workplace messages into trackable tasks. It is a frontend-only React, TypeScript, and Vite app; tasks and chat history stay in browser localStorage. The local parser works without an account, API key, or backend.

## Development

Requirements: Node.js 20 or newer.

```sh
npm install
npm run dev
```

Open the local URL printed by Vite. The first browser launch seeds 12 sample commitments. Task edits and chat are saved locally and persist across reloads.

## Production build

```sh
npm run build
npm run preview
```

The static production output is written to `dist/`.

## Deploy

Import this repository into Vercel or Netlify and use `npm run build` as the build command and `dist` as the publish directory. No environment variables or server functions are required. Both platforms provide SPA fallback for this single-screen app; if deploying to another static host, configure unknown routes to serve `/index.html`.

## Privacy and optional AI

Local parsing is always available. The settings panel describes an optional Gemini mode, but this build keeps parsing local; it does not send data or keys to an external service. Do not enter a key unless a future Gemini integration is enabled.
