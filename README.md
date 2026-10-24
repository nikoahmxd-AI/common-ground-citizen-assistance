# Common Ground — Citizen Assistance Prototype

A responsive frontend prototype for a hackathon project. It demonstrates a citizen dashboard, local issue reporting, request tracking, a service guide, demo alerts, and a small local help assistant.

## Run locally

```bash
npm install
npm run dev
```

To create a production build, run `npm run build`. Preview it with `npm run preview`.

## Project files

- `src/App.tsx` contains the React interface and demo interactions.
- `src/main.tsx` mounts the React app, and `src/styles.css` contains its styles.
- `preview.html` is a separate, dependency-free preview for opening the prototype directly as a local file. It mirrors the core demo flows and is maintained separately from the React app.

## Publish with GitHub Pages

The workflow in `.github/workflows/pages.yml` builds and deploys the site on each push to `main`. In the repository settings, set **Pages → Build and deployment → Source** to **GitHub Actions**. The first successful workflow run publishes the site URL in its deployment summary.

## Prototype scope

- Reporting creates a `DEMO-` reference and stores the record in this browser's `localStorage`. Selected photos are previewed locally and never uploaded.
- Tracking includes one sample request (`DEMO-24A7KQ`) with simulated Submitted, Assigned, and In Progress updates.
- Service guide entries, alerts, and help responses are sample content. The service guide makes no eligibility or procedural claims; alerts are fictional and not current or verified. No official sources have been verified or connected.
- There is no backend, government department connection, live alert feed, live AI, authentication, or real complaint submission.
- English and Tamil are available for navigation, the dashboard, and the main report and tracking flows. Other guide content is in English sample copy.

This project is frontend-only and uses demo information. Do not enter private or sensitive information.

Open `preview.html` directly for a no-install preview. When opened as a local file, `index.html` redirects to that preview. The React app is served through Vite after dependencies are installed.

## Future possibilities

Verified sources for a selected jurisdiction, approved government integrations, a staff dashboard, map-assisted reporting, voice support, and a verified alert feed are future possibilities. None are active in this prototype.
