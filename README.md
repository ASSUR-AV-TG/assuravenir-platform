# LES INDISPENSABLES

Projet Next.js + Tailwind + NextAuth + Prisma(Postgres) + Stripe

## Setup local
1. Copier `.env.example` → `.env` et remplir les valeurs
2. Installer les dépendances : `npm install`
3. Générer Prisma client et migrations :
   - `npx prisma generate`
   - `npx prisma migrate dev --name init`
4. Lancer le projet : `npm run dev`

## Deployment
- Sur Vercel, importer le repo GitHub
- Ajouter les variables d’environnement sur Vercel