# Simple Todo Application (React)

This repository contains a simple, responsive Todo application built with React. The app is currently **frontend-only** and runs on port **3000** in development.

## Features

The intended core Todo experience includes adding tasks, marking them complete or incomplete, deleting tasks, filtering by status (all, active, completed), and persisting tasks to local storage for a lightweight “no-backend” workflow.

The current frontend codebase also includes a basic light/dark theme toggle as part of the UI template.

## Project Structure

The React app lives under:

- `frontend/`: React application (Create React App)

## Getting Started

### Prerequisites

- Node.js (recommended: current LTS)
- npm

### Install and run

```bash
cd frontend
npm install
npm start
```

Then open:

- http://localhost:3000

## Environment Variables

This project supports a set of `REACT_APP_*` environment variables for configuration. Since the app is currently frontend-only, some of these may not be used yet, but they are available for future integration.

You can place these in `frontend/.env` (Create React App requires `REACT_APP_` prefix).

Supported keys:

- `REACT_APP_API_BASE`
- `REACT_APP_BACKEND_URL`
- `REACT_APP_FRONTEND_URL`
- `REACT_APP_WS_URL`
- `REACT_APP_NODE_ENV`
- `REACT_APP_NEXT_TELEMETRY_DISABLED`
- `REACT_APP_ENABLE_SOURCE_MAPS`
- `REACT_APP_PORT`
- `REACT_APP_TRUST_PROXY`
- `REACT_APP_LOG_LEVEL`
- `REACT_APP_HEALTHCHECK_PATH`
- `REACT_APP_FEATURE_FLAGS`
- `REACT_APP_EXPERIMENTS_ENABLED`

## Scripts

From `frontend/`:

- `npm start`: Run the development server
- `npm test`: Run tests
- `npm run build`: Create a production build
- `npm run eject`: Eject from CRA (one-way)

## Notes

This repository does not include a database container. If backend support is added later, the environment variables above provide a place to configure base URLs and WebSocket endpoints.
