# Generative-AI-for-Demystifying-Legal-Documents-
Simplification of legal document through generative AI , web application is visually stunning and highly functional user interface created using google cloud console 
-----------------------------------------------------------------------------------------------------------------------------

# Legal-Lawyer-AI

A Generative AI-powered application designed to demystify and analyze legal documents. Upload any legal document and receive instant, AI-driven insights to simplify complex legal jargon.

## Features

- Upload and analyze legal documents (PDFs)
- AI-powered clause extraction and document generation
- Secure and confidential document handling
- Real-time feedback through toast notifications
- Built with Next.js 13 App Router, TypeScript, Tailwind CSS, and Google Cloud Vertex AI integration

## Technology Stack

- Next.js (App Router + Turbopack)
- TypeScript
- Tailwind CSS
- Google Cloud Vertex AI API
- Supabase for file storage and backend API
- React Context & Custom Hooks for state management
- Radix UI for accessible UI components

## Getting Started

### Prerequisites

- Node.js (v18 or newer)
- Google Cloud Project with Vertex AI enabled and billing configured
- Supabase project for file uploads with keys ready
- `.env.local` file with the following keys:

-----------------------------------------------------------------------------------------------------------------------------

GOOGLE_API_KEY=your_google_api_key_here
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url_here
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key_here

-----------------------------------------------------------------------------------------------------------------------------

## Legal-Lawyer-AI/
 ### ├── public/                # Static assets (favicon.jpg, images, fonts)
 ### ├── src/
 ### │   ├── app/               # Entry point, routing, layouts
 ### │   │   ├── layout.tsx
 ### │   │   ├── page.tsx
 ### │   │   └── ...
 ### │   ├── components/        # Reusable UI (toasts, modals, forms)
 ### │   │   ├── Toast.tsx
 ### │   │   └── ...
 ### │   ├── pages/             # API routes, custom pages (if not using /app)
 ### │   │   └── api/           # Server API route handlers for AI calls
 ### │   ├── features/          # Domain logic (Legal document generators, clause parsing, etc.)
 ### │   │   ├── DocumentGenerator/
 ### │   │   └── ClauseParser/
 ### │   ├── hooks/             # Custom React hooks (useToast.tsx, etc.)
 ### │   ├── utils/             # Utility functions (formatting, parsing)
 ### │   │   ├── utils.tsx
 ### │   │   └── supaBaseClient.ts
 ### │   ├── services/          # API clients, Google Cloud, Vertex AI connectors
 ### │   ├── context/           # React Context providers (global state)
 ### │   ├── store/             # State management (Redux, Zustand if used)
 ### │   ├── styles/            # Global and component styles (globals.css)
 ### │   ├── config/            # Configuration (API keys, endpoints)
 ### │   ├── constants/         # Static values, roles, message strings
 ### │   └── types/             # TypeScript interfaces and types
 ### ├── .env.local             # Environment variables
 ### ├── next.config.js         # Next.js configuration
 ### ├── package.json           # Project metadata
 ### ├── tsconfig.json          # TypeScript configuration
 ### └── README.md              # Project documentation

-----------------------------------------------------------------------------------------------------------------------------

### to enter into the project and install libraries:
### npx create-next-app Legal-Lawyer-AI --typescript

## Which linter would you like to use? › - Use arrow-keys. Return to submit.
### ❯   ESLint - More comprehensive lint rules
   ### Biome
   ### None        what should u choose

### For most professional AI, TypeScript, and Next.js projects, ESLint is recommended because it offers comprehensive linting, plugin support, strong TypeScript integration, and is widely used in industry. Biome is modern, super fast, and combines linting and formatting in one, but its extensibility and plugin ecosystem are not as mature, and some formatting/linting features or integrations may be limited for large scale or legacy projects.

### What to choose?
### For maximum compatibility, configurability, and reliability—ESLint.
### For a simple, fast, all-in-one tool and if you want the latest technology—Biome.
### For most use cases, select ESLint unless project requirements or your team specifically prefer Biome.

## Would you like to use Tailwind CSS? › No / Yes ( a choice to make )
### Tailwind CSS is already used in your project, as indicated by the "globals.css" file importing Tailwind and various className usages that match Tailwind's utility classes in your React components.

### What should you choose?
### For the question Would you like to use Tailwind CSS?
### Choose: Yes

## Would you like to use App Router? (recommended) › No / Yes

### You should choose: Yes for using the App Router.
### Your project already includes files like src/app/layout.tsx and src/app/page.tsx, which are part of Next.js's App Router structure. The App Router is the modern, recommended routing and layout system for all new Next.js projects, enabling advanced features, better flexibility, and improved scalability for apps like Legal-Lawyer-AI. 
-----------------------------------------------------------------------------------------------------------------------------

### cd Legal-Lawyer-AI
### npm install

### to run the local project:

### bash
### npm install
### npm run dev

### npx create-next-app Legal-Lawyer-AI --typescript
### cd Legal-Lawyer-AI

## Create core folders following modern scalable structure
### mkdir -p public src/app src/components src/pages/api src/features/DocumentGenerator \
### src/features/ClauseParser src/hooks src/utils src/services src/context src/store \
### src/styles src/config src/constants src/types

## App and routing
### touch src/app/layout.tsx src/app/page.tsx

## Components (UI)
### touch src/components/Toast.tsx

## API routes
### touch src/pages/api/ai.ts

## Features - legal document and clause parsing modules
### touch src/features/DocumentGenerator/index.ts
## touch src/features/ClauseParser/index.ts

## Custom React hooks
### touch src/hooks/useToast.tsx

## Utilities
### touch src/utils/utils.tsx src/utils/supaBaseClient.ts

## Services (API, Google Cloud, Vertex AI connectors)
### touch src/services/vertexAI.ts

## Context (React providers)
### touch src/context/AppContext.tsx

## Store (global state files, e.g. if using Zustand/Redux)
### touch src/store/index.ts

## Style files
### touch src/styles/globals.css

## Config and constants
### touch src/config/index.ts src/constants/index.ts

## Types (TypeScript interfaces)
### touch src/types/index.ts

## Add the default favicon and any images to public
## (Example, if you have a file favicon.jpg)
### mv ../favicon.jpg public/

## Project root files (if missing)
### touch README.md          # Documentation
### touch .env.local         # Local environment variables
### touch next.config.js     # Next.js configuration

## Ensure TypeScript config exists
### touch tsconfig.json      # TypeScript settings (included if not present from starter)

## Package metadata
### touch package.json       # If not created by npx (normally is)

## Yarn/NPM lock file
### touch yarn.lock          # If using yarn (already included if not removed)

## Add index files to folders for easy imports and scalability
### touch src/components/index.ts
### touch src/features/index.ts
### touch src/hooks/index.ts
### touch src/services/index.ts
### touch src/context/index.ts
### touch src/store/index.ts
### touch src/styles/index.ts
### touch src/config/index.ts
### touch src/constants/index.ts
### touch src/types/index.ts

## If not created, ensure api folder for additional backend endpoints
### mkdir -p src/pages/api

## If planning tests or storybook
### mkdir -p src/tests src/stories
### touch src/tests/index.test.ts
### touch src/stories/index.stories.ts

## Optional: For assets like fonts
### mkdir -p public/fonts

-----------------------------------------------------------------------------------------------------------------------------

## Open your browser and visit `http://localhost:3000` or `http://localhost:3001` to see the app in action.
-----------------------------------------------------------------------------------------------------------------------------

## Deployment

The app can be deployed to Google Cloud Run or any preferred platform supporting Next.js. Ensure environment variables are set accordingly in your deployment environment.

## Folder Structure Highlights

- `src/app/` - Application routes and layouts
- `src/components/` - Reusable UI components (Toast, Buttons, etc.)
- `src/features/` - Legal Document and Clause handling modules
- `src/hooks/` - Custom React hooks (useToast for notifications)
- `src/services/` - API clients, Google Cloud integration
- `src/utils/` - Helper functions and utilities
- `public/` - Static assets and SVG icons

## TO VIEW PROJECT 
### https://console.cloud.google.com/billing/015519-495D35-F849EE/credits/all?authuser=0&cloudshell=true&project=p1h25study
---

*Created by [SURAJ SINGH]*

