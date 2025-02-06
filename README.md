# React Project Setup Guide

## Project Initialization and Configuration

This guide walks you through creating a new React project with TypeScript using Vite and installing essential libraries.

## Prerequisites

- Node.js (recommended version 18.x or later)
- npm (Node Package Manager)

## Step-by-Step Setup

### 1. Create Vite React Project with TypeScript

Run the following command in your terminal:

```bash
npm create vite@latest web -- --template react-ts
```
![Zrzut ekranu 2025-02-06 141245](https://github.com/user-attachments/assets/a5b45fa3-ad22-4cec-aee7-6f44c96c84c7)

When prompted, make the following selections:
- ![Zrzut ekranu 2025-02-06 141253](https://github.com/user-attachments/assets/a0236aa0-b985-4523-ac4f-28273091650c)
- ![Zrzut ekranu 2025-02-06 141305](https://github.com/user-attachments/assets/320015ff-a1c1-461f-a5ed-a92711b614c7)
- ![Zrzut ekranu 2025-02-06 141318](https://github.com/user-attachments/assets/3f41dc8e-4955-429f-bcc6-d39a5b94fdc8)


### 2. Navigate to Project Directory

```bash
cd web
```

### 3. Install Project Dependencies

Run the following command to install all necessary libraries:

```bash
npm install @emotion/react @emotion/styled @microsoft/signalr @mui/icons-material @mui/material @mui/x-data-grid @tanstack/react-query @toolpad/core axios react-hook-form react-number-format react-router-dom vite-plugin-svgr
```

This command installs:
- Emotion for styling
- SignalR for real-time communication
- Material-UI components and icons
- Tanstack React Query for data fetching
- Axios for HTTP requests
- React Hook Form for form management
- React Number Format for number inputs
- React Router for navigation
- SVG import plugin for Vite

### 4. Upgrade Dependencies

```bash
npm upgrade
```

This ensures you have the latest compatible versions of your dependencies.

## Additional Configuration

### Vite Configuration

Update your `vite.config.ts` to include the SVG plugin:

```typescript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react-swc'
import svgr from 'vite-plugin-svgr'

export default defineConfig({
  plugins: [
    react(),
    svgr()
  ],
})
```
Update your `vite-env.d.ts` to include the SVG plugin:

```typescript
/// <reference types="vite/client" />
/// <reference types="vite-plugin-svgr/client" />
```

### Recommended VS Code Extensions

- ESLint
- Material Icon Theme

## Running the Project

### Development Server

```bash
npm run dev
```

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Project Structure

### At start
```
web/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── App.tsx
│   └── main.tsx
├── .eslintrc.cjs
├── .gitignore
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

### Our project structure
```
web/
├── public/
├── src/
│   ├── assets/
│   ├── pages/
│   ├── shared/
|       ├── auth/
|       ├── clients/
|       ├── components/
|       ├── helpers/
|       ├── hooks/
|       ├── router/
|       ├── theme/
|       └──values/
│   ├── index.css
│   ├── vite-env.d.ts
│   ├── App.tsx
│   └── main.tsx
├── .eslintrc.cjs
├── .gitignore
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

## Recommended Practices

- Use TypeScript for type safety
- Utilize React Query for data fetching and state management
- Implement component-based architecture
- Use Material-UI for consistent design
- Leverage React Router for navigation

## Troubleshooting

- Ensure Node.js and npm are up to date
- Clear npm cache if dependency issues occur: `npm cache clean --force`
- Reinstall dependencies if needed: `rm -rf node_modules && npm install`
