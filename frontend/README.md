# React Todo App (Frontend)

This folder contains the React frontend for a simple Todo application. The app runs locally on port **3000** by default.

## Features

The product goal for this frontend is a lightweight Todo experience with:

- Adding new todos
- Marking todos complete or incomplete
- Deleting todos
- Filtering by status (all, active, completed)
- Persisting todos in browser storage for a backend-free workflow
- Responsive, centered layout suitable for desktop and mobile

The current codebase also includes a light/dark theme toggle as part of the UI template.

## Tech Stack

This app is built with:

- React
- Create React App (`react-scripts`)
- Vanilla CSS (no UI framework)

## Getting Started

### Prerequisites

- Node.js (recommended: current LTS)
- npm

### Install dependencies

```bash
npm install
```

### Run the app

```bash
npm start
```

Then open:

- http://localhost:3000

## Environment Variables

Create React App only exposes environment variables prefixed with `REACT_APP_`. Create a `frontend/.env` file to override defaults.

The following keys are supported by the container configuration (some may not be used yet by the current frontend code, but are available for future API/WebSocket integration):

- `REACT_APP_API_BASE`: Base path for API requests (for example, `https://example.com/api`)
- `REACT_APP_BACKEND_URL`: Backend base URL (if/when a backend is introduced)
- `REACT_APP_FRONTEND_URL`: Public frontend URL (useful for constructing absolute links)
- `REACT_APP_WS_URL`: WebSocket URL (if/when realtime is introduced)
- `REACT_APP_NODE_ENV`: Runtime environment indicator
- `REACT_APP_NEXT_TELEMETRY_DISABLED`: Telemetry toggle (reserved)
- `REACT_APP_ENABLE_SOURCE_MAPS`: Enable/disable sourcemaps in builds
- `REACT_APP_PORT`: Preferred port for the dev server (default is typically 3000)
- `REACT_APP_TRUST_PROXY`: Proxy trust toggle (reserved)
- `REACT_APP_LOG_LEVEL`: Logging verbosity level (reserved)
- `REACT_APP_HEALTHCHECK_PATH`: Healthcheck path (reserved)
- `REACT_APP_FEATURE_FLAGS`: Feature flag configuration (reserved)
- `REACT_APP_EXPERIMENTS_ENABLED`: Experiment toggle (reserved)

## Available Scripts

- `npm start`: Starts the dev server
- `npm test`: Runs tests (CRA test runner)
- `npm run build`: Builds a production bundle to `build/`
- `npm run eject`: Ejects CRA configuration (one-way)

## Troubleshooting

If you change `.env` values while the dev server is running, you usually need to restart `npm start` for changes to take effect.
