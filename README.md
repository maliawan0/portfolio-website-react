# Portfolio Website

My personal portfolio site — React + Vite + Tailwind CSS. Built for a Web Programming assignment and kept as my live portfolio.

## Features

- **Routed pages** — Home, About, Projects, Contact, plus a data-entry view
- **Data-driven project cards** — projects come from [`src/assets/data.json`](src/assets/data.json), so adding one is a JSON edit rather than a component change
- **Animated gradient background** — custom `Gradient` component
- **Responsive layout** throughout, via Tailwind

## Stack

React 18 · Vite · React Router · Tailwind CSS · ESLint

## Layout

```
src/
  Pages/       # Home, About, Projects, Contact, DataEntry
  Components/  # Navbar, Footer, ProjectCard, Gradient
  assets/
    data.json  # project entries rendered by ProjectCard
  main.jsx     # entry
```

## Running it locally

```bash
npm install
npm run dev
```

Vite serves at `http://localhost:5173`.

```bash
npm run build     # production build to dist/
npm run preview   # preview the build
npm run lint      # ESLint
```

## Adding a project

Append an entry to `src/assets/data.json` — the Projects page maps over it and renders a `ProjectCard` for each. No component changes needed.
