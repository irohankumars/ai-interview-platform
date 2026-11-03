# prepwise · AI interview practice

A responsive frontend prototype for practicing technical interviews. Sign-in, question generation, and feedback are simulated locally; no OAuth, AI, transcription, or backend connection is configured.

## Run locally

```sh
npm install
npm run dev
```

Open the local address printed by Vite. Use the demo Google sign-in button to enter the app. To create a production bundle, run `npm run build`.

## Frontend structure

- `src/App.jsx` — page flows and shared UI
- `src/data/mockData.js` — candidate, interview prompts, and seeded debriefs
- `src/services/interviewService.js` — replaceable mock data and auth services
- `src/styles.css` — responsive design system

Live interview responses are stored locally in browser storage. Microphone recording requires browser permission and a secure context (localhost is supported). Uploaded resumes are validated in-browser and not sent anywhere.
