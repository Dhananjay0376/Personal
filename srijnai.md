🏗️ Architecture & Monorepo
Architecture: Monorepo using npm Workspaces (
package.json
)
Workspace Packages:
apps/web
 — Next.js frontend web application
apps/api
 — Node.js / Vercel Serverless API backend
packages/db
 — Shared database schema and migrations
packages/ai
 — Shared AI provider & prompt logic
packages/ui
 & 
packages/types
 — UI component primitives and TypeScript type definitions
🎨 Frontend
Framework: Next.js 16 (App Router)
Language: TypeScript 5.9 & React 19
Styling: Tailwind CSS v4 & PostCSS
3D Graphics & Visuals: Three.js (@react-three/fiber, @react-three/drei, @react-three/postprocessing)
Animations: Framer Motion (framer-motion)
Icons: Lucide React (lucide-react)
🗄️ Backend & Database
Runtime: Node.js (Serverless Function setup via Vercel)
Database: Supabase (PostgreSQL)
ORM & Query Builder: Drizzle ORM with Drizzle Kit (drizzle-kit, pg)
🔐 Authentication & Security
User Authentication: Clerk (@clerk/nextjs)
🤖 AI Engine & LLM Integrations
Multi-LLM Fallback Architecture:
Groq
Google Gemini
OpenRouter
Anthropic (fallback capabilities)
🚀 Deployment & Tooling
Hosting / Deployment: Vercel (Frontend & Serverless Functions)
Environment Configuration: Dotenv
1:33 PM




