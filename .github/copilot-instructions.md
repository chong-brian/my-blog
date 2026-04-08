# Copilot Instructions for this Repository

## Project context
- This is a React 19 app built with Vite.
- Routing uses `react-router-dom` v7.
- Tests use Vitest + Testing Library (`jsdom` environment, global test APIs enabled).
- JavaScript only (no TypeScript).

## Code style and conventions
- Prefer function components and hooks.
- Match existing formatting: single quotes and semicolons.
- Keep component logic readable and straightforward; avoid over-abstraction.
- Use clear, descriptive names for components, props, and helper functions.
- Preserve existing folder conventions:
  - Reusable UI pieces in `src/components/`
  - Route-level screens in `src/pages/`

## Routing guidance
- Follow the route structure defined in `src/App.jsx`.
- When adding new pages, wire routes in `src/App.jsx` and keep fallback behavior (`*`) intact.
- Keep navigation updates aligned with `src/NavBar.jsx` when route changes affect site navigation.

## Data and API usage
- Use relative `/api/...` endpoints for app requests so Vite dev proxy works.
- Assume backend runs at `http://localhost:8000` in development via proxy config.
- Handle async loading and error states explicitly in UI.

## Testing expectations
- Use Vitest APIs (`describe`, `it`/`test`, `expect`, `vi`) and Testing Library for component behavior.
- Prefer user-facing assertions (visible text, roles, interactions) over implementation details.
- Put tests next to source files or follow existing test placement patterns.
- For changed behavior, add or update tests when practical.

## Change safety
- Keep diffs focused on the requested task.
- Avoid unrelated refactors and formatting-only churn.
- When editing existing files, preserve current public behavior unless the task requests a change.

## Useful commands
- Install deps: `npm install`
- Start dev server: `npm start`
- Run tests: `npm test`
- Build production bundle: `npm run build`
- Preview production build: `npm run preview`
