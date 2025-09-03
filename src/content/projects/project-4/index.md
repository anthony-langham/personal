---
title: "Care Engineering"
description: "Ambient Scribe and Decision Support SaMD."
date: "June 18 2025"
demoURL: "https://www.care.engineering"
repoURL: "https://github.com/anthony-langham"
---

Live transcription tool that predicts likely diagnoses and prompts the next 3 most relevant follow up questions to narrow further.

![Care Engineering](/AmbientScribePlus.png)

A React-based medical assistant application that uses OpenAI's realtime API for voice interactions and provides clinical note extraction, diagnostic suggestions, and structured medical documentation.

Project Structure
Frontend: React SPA with Vite build system
Backend: Express.js server with OpenAI realtime API integration
Deployment: AWS SST framework
Database: DynamoDB (via SST)
Authentication: JWT-based with bcrypt password hashing
Key Components
Client (/client/)
App.jsx - Main application component
AuthWrapper.jsx - Authentication wrapper
DiagnosisPanel.jsx - Medical diagnosis interface
TranscriptionPanel.jsx - Real-time transcription display
StructuredNotePanel.jsx - Clinical note formatting
SuggestedQuestionsPanel.jsx - AI-generated follow-up questions
SessionControls.jsx - Audio session management
Server (/server.js)
Express server with Vite middleware
OpenAI realtime API integration
JWT authentication endpoints
Clinical note processing APIs
Services (/services/)
clinicalNoteExtractor.js - Extracts structured clinical data
diagnosticEngine.js - Provides diagnostic suggestions
Infrastructure (/stacks/)
API.ts - API Gateway configuration
Database.ts - DynamoDB tables
Web.ts - Static site hosting
Available Commands
Development
npm run dev - Start development server
npm run sst:dev - Start SST development environment
Build & Deploy
npm run build - Build client and server
npm run build:client - Build React client only
npm run build:server - Build server for production
npm run sst:deploy - Deploy to AWS
npm run sst:remove - Remove AWS resources
Code Quality
npm run lint - Run ESLint with auto-fix
Environment Variables
Required environment variables:

OPENAI_API_KEY - OpenAI API key for realtime sessions
JWT_SECRET - Secret for JWT token signing
SESSION_SECRET - Express session secret
Authentication
The app uses JWT tokens for authentication with the following endpoints:

POST /login - User login
POST /register - User registration
Protected routes require Authorization: Bearer <token> header
OpenAI Integration
Uses OpenAI's realtime API model: gpt-4o-realtime-preview
Voice mode: "verse"
Generates ephemeral tokens for client-side connections
Supports real-time audio transcription and responses
Medical Features
Clinical Note Extraction: Processes conversation transcripts into structured medical notes
Diagnostic Engine: Provides AI-powered diagnostic suggestions
Structured Documentation: Formats clinical encounters into standardized formats
Suggested Questions: Generates relevant follow-up questions for medical interviews
UI Framework
shadcn/ui Integration (Updated 2025-01-07)
Migrated from custom components to shadcn/ui component library
Consistent design system with modern card-based layouts
Professional medical application styling
Key UI Components
AppLayout.jsx - Main layout wrapper with sidebar integration
AppSidebar.jsx - Collapsible sidebar navigation with medical-focused sections
All panels now use shadcn/ui Cards, ScrollAreas, and Badges
Responsive design with mobile support via use-mobile hook
Layout Structure
Sidebar Navigation: Medical console navigation with user profile and logout
Main Content: Full-width responsive grid layout
No Header: Clean design with all controls in sidebar
User Management: Logout functionality integrated in sidebar footer
shadcn/ui Components Used
Card, CardContent, CardHeader, CardTitle
Button with variants
Badge
ScrollArea
Avatar
Separator
Sidebar components
Development Notes
Uses ES modules ("type": "module" in package.json)
React 18 with modern hooks
shadcn/ui + Tailwind CSS for consistent design system
Vite for fast development and building
TypeScript support for infrastructure code
