The Challenge:
Modern luxury e-commerce demands an engaging visual experience, dynamic content updates, and instant multi-channel ordering (Web + WhatsApp)—without the high overhead, performance bottlenecks, or vendor lock-in of traditional monolithic storefronts. The goal was to build a full-stack e-commerce platform capable of handling real-time catalog sync, atomic checkout transactions, variant-level stock protection, automated shipping dispatch, and immersive 3D product previews while supporting single-codebase deployment to web and native mobile apps.

The Solution:
Engineered a decoupled, full-stack architecture powered by a React + Vite frontend integrated with Three.js for interactive 3D product galleries. Implemented Sanity CMS with dynamic fallbacks for zero-downtime catalog management, alongside Supabase PostgreSQL with custom RPC functions for atomic multi-table checkout writes (orders, order_items, customers) and automated stock triggers. Integrated NimbusPost API for real-time pincode serviceability and shipping manifest creation, protected admin inventory operations via Row-Level Security (RLS), and packaged the entire application for native Android deployment using Capacitor.


Key Highlights / Outcomes:

Zero-Downtime Catalog & Content Sync: Seamless headless integration with Sanity CMS and fallback architecture, enabling non-technical team members to update product lines, collections, and pricing instantly without code redeployments.
100% Transactional Integrity Across Channels: Built atomic database procedures using Supabase PostgreSQL RPC, eliminating partial writes and race conditions across hybrid Web and WhatsApp checkout flows.
Automated Stock Protection & Admin Security: Enforced real-time variant inventory reservations upon order payment, automatic stock restoration on cancellations, and protected admin control panel access via Row-Level Security (RLS).
Automated Shipping & Fulfillment: Integrated NimbusPost API for instant buyer PINCODE serviceability checks, automated courier selection, and 1-click shipment manifest creation, eliminating manual logistics dispatch bottlenecks.
Immersive 3D Product Engagement: Built touch-optimized 3D jewelry showcases powered by Three.js, elevating customer engagement and visual fidelity for luxury items without compromising page load speeds.
Single-Codebase Cross-Platform Build: Leveraged Capacitor CLI over the React + Vite codebase to package native Android mobile apps, achieving 100% code reuse between web and mobile platforms.
