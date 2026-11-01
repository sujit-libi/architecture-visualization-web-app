# Project Guide

## Overview

- This is a TypeScript application built with React 19 and React Router v8.
- The app uses server-side rendering by default (`react-router.config.ts`).
- Routes are declared in `app/routes.ts`; route modules live in `app/routes/`.
- Shared components live in `components/`, with reusable UI components in `components/ui/`.
- Tailwind CSS v4 is configured through Vite. Global styles and theme tokens are in `app/app.css`.

## Commands

- `npm run dev` starts the development server.
- `npm run typecheck` runs React Router type generation and TypeScript checks.
- `npm run build` creates the production build.

There is no test script currently defined in `package.json`.

## Working Conventions

- Follow the existing TypeScript and React patterns in nearby route modules and components.
- Use React Router route modules and generated route types for route-specific metadata and APIs.
- Keep shared UI in `components/`; use the existing global theme and Tailwind setup for styling.
- Preserve server rendering unless a task explicitly requires changing the rendering mode.
- Keep changes focused and run `npm run typecheck` or `npm run build` when relevant.
