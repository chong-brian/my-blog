# My Blog

A React blog application built with [Vite](https://vitejs.dev/), [React 19](https://react.dev/), and [React Router v7](https://reactrouter.com/).

## Tech Stack

- **Vite** — build tool and dev server
- **React 19** — UI library
- **React Router v7** — client-side routing

## Getting Started

### Prerequisites

- Node.js (v18+)
- A backend API server running on `http://localhost:8000`

### Install Dependencies

```bash
npm install
```

## Available Scripts

### `npm start`

Runs the app in development mode. Open [http://localhost:5173](http://localhost:5173) to view it in the browser.

The page will hot-reload on edits.

### `npm run build`

Builds the app for production to the `dist` folder. The build is minified and filenames include content hashes.

### `npm run preview`

Serves the production build locally for previewing before deployment.

## Project Structure

```
├── index.html                  # Vite entry HTML
├── vite.config.js              # Vite configuration
├── public/                     # Static assets
└── src/
    ├── index.jsx               # App entry point
    ├── App.jsx                 # Root component and routes
    ├── NavBar.jsx              # Navigation bar
    ├── components/
    │   ├── AddCommentForm.jsx
    │   ├── ArticlesList.jsx
    │   ├── CommentsList.jsx
    │   └── UpvotesSection.jsx
    └── pages/
        ├── HomePage.jsx
        ├── AboutPage.jsx
        ├── ArticlesListPage.jsx
        ├── ArticlePage.jsx
        ├── NotFoundPage.jsx
        └── article-content.js
```

## API Proxy

The dev server proxies `/api` requests to `http://localhost:8000`. Make sure your backend is running before starting the app.

## Learn More

- [Vite Documentation](https://vitejs.dev/guide/)
- [React Documentation](https://react.dev/)
- [React Router Documentation](https://reactrouter.com/)
