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




 Srijan AI (सृजन — the art of creation)
Description:
Srijan AI is an intelligent monthly content planning platform designed for creators across Instagram, YouTube, LinkedIn, and X (Twitter). By providing a niche, target platform, tone, and language, creators receive a platform-native, 30-day interactive content calendar complete with visual hooks, captions, hashtag sets, thread outlines, and call-to-actions tailored to each channel's audience behavior.

The Challenge:
Content creators rarely struggle with making content — they struggle with planning it consistently without hitting creative burnout. Existing AI generators often produce generic, one-size-fits-all copy, lack platform awareness, and rely on single LLM APIs that frequently break or hit rate limits during peak usage. Additionally, creators need historical context so that generated themes evolve naturally month-over-month.

The Solution:
Engineered as a high-performance monorepo (using npm Workspaces) featuring a Next.js 16 (App Router) frontend, a Node.js serverless backend API, and a shared database layer powered by Supabase PostgreSQL and Drizzle ORM.

Multi-LLM Fallback Engine: Built an intelligent API proxy chain (Groq → Gemini → OpenRouter → Anthropic) to seamlessly handle failures, rate limits, or outages without interrupting the user experience.
Platform-Native Content Engine: Programmed platform-tuned prompt strategies to generate structured, platform-specific outputs (e.g., visual hooks for Instagram, thread structures for X, thought-leadership framing for LinkedIn).
3D Interactive Experience: Implemented Three.js rendering (@react-three/fiber & @react-three/drei) alongside modern glassmorphic styling and Framer Motion animations for an immersive creator interface.
Production Auth & Security: Integrated Clerk authentication to manage secure multi-user onboarding and persistent creator profiles.
Key Highlights/Outcomes:

Zero Downtime Content Generation: Multi-LLM fallback mechanism ensures near-100% operational reliability even when individual AI provider endpoints encounter rate limits or degradation.
Platform-Tuned Outputs: Generates specialized content structures for 4 major platforms (Instagram, YouTube, LinkedIn, X) rather than generic text templates.
Scalable Monorepo Architecture: Modular code separation across 
apps/web
, 
apps/api
, 
packages/db
, and 
packages/ai
.
Instant Calendar Automation: Reduces full monthly content plan creation time from hours/days down to seconds.
Links:

Live Demo: (https://srijan-ai-web-wy1m.vercel.app/)
GitHub Repository: github.com/Dhananjay0376/SrijanAI
