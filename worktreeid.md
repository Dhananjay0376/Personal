Title: WorkTree ID
Category: Full-Stack
Tech Stack: React 19, TypeScript, Vite, React Router, Tailwind CSS, Firebase (Auth & Firestore), IndexedDB, Framer Motion, Lucide Icons
Description: WorkTree ID is a collaborative project management and visual node-tree mapping web application. It enables users to organize complex projects as nested, hierarchical work trees (root -> branch -> stem -> leaf -> fruit), manage user profiles, and collaborate with team members through invite systems and public/private visibility controls.
The Challenge: Traditional task managers struggle to clearly visualize deep hierarchical node dependencies and handle rich media attachments without latency. The challenge was building an interactive, real-time collaboration environment with dual visualization formats (tree lists and visual horizontal graphs), robust state history (undo/redo), low-latency rendering, and seamless cloud synchronization.
The Solution:
Designed a recursive, typed node architecture with support for multiple content formats (normal text, rich notes, links, images, and videos).
Implemented a hybrid storage pattern pairing localStorage and IndexedDB for instant browser-local UI updates and media caching with Firebase Auth and Firestore for cloud sync and invite notifications.
Built two dynamic views: a responsive structured tree editor with inline controls and a visual horizontal graph layout powered by Framer Motion.
Engineered identity management with unique username registration, public/private profile controls, and collaboration invite pipelines (project_invite and team_up).
Key Highlights/Outcomes:
Hierarchical Node Breakdown: Intuitive multi-level project tree mapping (root -> branch -> stem -> leaf -> fruit).
Dual Visualization Modes: Seamlessly switch between structured tree list editing and interactive horizontal node graphs.
Hybrid Offline-First Sync: Ultra-responsive local state updates backed by Firestore cloud persistence and authentication.
Granular Collaboration & Roles: Invitation system for project collaborators with view/edit access controls and profile team sections.
Rich Node Content & History: Native support for image/video attachments, resizable note blocks, search/filtering, and full undo/redo action history.
Links: 
GitHub Repository: https://github.com/Dhananjay0376/WorkTree-iD
Live link:https://worktree-id.web.app/
