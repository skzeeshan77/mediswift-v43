MEDISWIFT V4.3 - VERCEL + POSTGRESQL READY
==========================================

This version replaces local JSON persistence with PostgreSQL so login, profile,
cart, orders, appointments and messages can persist on a serverless deployment.

FILES ADDED/CHANGED
- api/index.js              Vercel function entrypoint
- vercel.json               Rewrites /api/* to Express
- package.json              Root Node dependencies
- .env.example              Database variable template
- .gitignore                Excludes secrets and node_modules
- backend/server.js         PostgreSQL-backed API; still runs locally

VERCEL ENVIRONMENT VARIABLE REQUIRED
DATABASE_URL=<your hosted PostgreSQL/Neon connection string>
SESSION_TTL_DAYS=30   (optional)

GITHUB
Upload the CONTENTS of this folder to your repository root.
Do not upload node_modules or a real .env file.

LOCAL TEST (optional)
1. Copy .env.example to .env and fill DATABASE_URL.
2. PowerShell at project root: npm.cmd install
3. PowerShell: $env:DATABASE_URL="your connection string"
4. PowerShell: node backend/server.js
5. Open http://localhost:3000

DATABASE TABLES
The backend creates required tables automatically on first /api request.
