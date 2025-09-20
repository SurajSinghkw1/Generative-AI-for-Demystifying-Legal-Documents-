# Generative-AI-for-Demystifying-Legal-Documents-
Simplification of legal document through generative AI , web application is visually stunning and highly functional user interface created using google cloud console 

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

GOOGLE_API_KEY=your_google_api_key_here
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url_here
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key_here

### cd Legal-Lawyer-AI
### npm install

### to run the local project:

## bash
### npm install
### npm run dev


Open your browser and visit `http://localhost:3000` or `http://localhost:3001` to see the app in action.

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

## Contributing

Contributions are welcome! Please feel free to submit issues and pull requests for improvements or fixes.

## License

This project is licensed under the MIT License.

---

*Created by [Your Name]*

