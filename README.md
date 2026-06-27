# final-year-proj

A final year project web application built with a modern React + TypeScript frontend stack.

## Overview

This repository contains the main frontend application and related project folders.  
The root app uses Vite for development/build tooling and Tailwind-based UI components.

## Tech Stack

- React 18
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui (Radix UI-based components)
- Vitest + Testing Library

## Getting Started

### Prerequisites

- Node.js (recommended: current LTS)
- npm

### Installation

```bash
git clone https://github.com/mrkrishna225/final-year-proj.git
cd final-year-proj
npm ci
```

### Run Locally

```bash
npm run dev
```

## Available Scripts

- `npm run dev` - Start the Vite dev server
- `npm run build` - Build for production
- `npm run build:dev` - Build using development mode
- `npm run preview` - Preview the production build locally
- `npm run lint` - Run ESLint
- `npm run test` - Run Vitest once
- `npm run test:watch` - Run Vitest in watch mode

## Editing / Development Options

- Use your local IDE/editor (recommended): update files and run scripts from this repository root.
- Edit directly in GitHub for quick documentation or small code changes.
- Use GitHub Codespaces for a cloud development environment.

## Deployment Notes

This project builds to static frontend assets using `npm run build` (output in `dist/`).  
Deploy the `dist/` output to any static hosting platform (for example: Vercel, Netlify, GitHub Pages, or an Nginx-based server).
