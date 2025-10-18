# AssurAvenir — Plateforme Apprenant

Prototype Next.js + Tailwind + NextAuth + Prisma(Postgres) + Stripe
Includes admin page, student dashboard, checkout webhook.

## Setup (local)

1. Copy `.env.example` to `.env` and fill values (DATABASE_URL, NEXTAUTH_SECRET, STRIPE keys).
2. Install: `npm install`
3. Generate Prisma client and run migrations:
   - `npx prisma generate`
   - `npx prisma migrate dev --name init`
4. Run dev: `npm run dev`
5. To test Stripe webhooks locally: `stripe listen --forward-to localhost:3000/api/stripe/webhook`

## Deploy
Recommended: Vercel (frontend + API routes). Use managed Postgres (Railway, Supabase, Neon).
Set environment variables in the deployment dashboard.

