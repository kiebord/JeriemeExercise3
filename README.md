# Notes v8 — Swiss Typography

A standalone Next.js notes app with strict grid typography and vivid red geometry.

## Run it

```bash
npm install
npm run dev
```

Open `http://localhost:3000`. For verification, run:

```bash
npm run typecheck
npm run build
```

## Requirement mapping

- `app/page.tsx`: `useState` state, `useEffect` load/save/duplicate checks, validation, feedback, confirmation, and localStorage error handling.
- `components/NoteItem.tsx`: separate note row component with edit and delete actions.
- Add, view, edit, and delete are all functional. Titles are normalized with `trim()`, lowercase conversion, and repeated-whitespace collapsing; editing excludes the current note ID.
- Storage key: `notefolio-notes-swiss-v8`.
- `app/globals.css`: Swiss grid layout plus desktop, tablet, and 360px-friendly responsive rules, focus states, readable contrast, and touch-sized controls.
- No backend, login, or remote data is used.
