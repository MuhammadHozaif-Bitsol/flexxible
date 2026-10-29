# Flexxible

An early-stage Next.js app for showcasing developer projects ("Showcase and develop remarkable dev projects"). So far it has the site layout, a navbar and a footer; the home page and the auth, button and profile components are placeholders.

## Tech stack

- Next.js 16 (App Router, React Compiler)
- React 19, TypeScript
- Tailwind CSS 4
- Installed but not yet used in the code: next-auth, jsonwebtoken, graphql-request, @grafbase/sdk, cloudinary, @headlessui/react

## Features

- Root layout with the Inter font, `Navbar` and `Footer`
- Navbar with the logo and links from `constants/index.ts` (shown on extra-large screens); all links currently point to `/`
- Footer with seven link columns and a copyright line
- `constants/index.ts` also defines a list of project category filters (Frontend, Backend, Mobile, and others) that is not rendered yet
- `common.types.ts` defines TypeScript types for the planned data (projects, users, sessions)

## Getting started

```bash
npm install
npm run dev      # start the dev server at http://localhost:3000
npm run build    # production build
npm run start    # run the production build
npm run lint     # run ESLint
```

No environment variables are read by the code yet.

## Project structure

```
app/                 Root layout, home page, global styles
components/          Navbar, Footer, and placeholder AuthProviders, Button, ProfileMenu
constants/index.ts   Nav links, category filters, footer links
common.types.ts      Shared TypeScript types
public/              Logos and icons
```

## Notes

This project uses a recent Next.js version whose APIs may differ from older releases; see `AGENTS.md`.
