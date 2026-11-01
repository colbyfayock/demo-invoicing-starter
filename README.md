# Demo Invoice App Starter

A full-stack Next.js invoicing demo where Clerk-authenticated users manage invoices stored per user in Neon Postgres through Drizzle.

## Use this template

```bash

```

## Local setup

Install dependencies, then create a Clerk application and a Neon Postgres database:

```bash
npm install
```

Set these values in `.env.local`:

```dotenv
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<Clerk publishable key>
CLERK_SECRET_KEY=<Clerk secret key>
DATABASE_URL=<Neon Postgres connection string>
# Optional, for the Clerk webhook endpoint
CLERK_WEBHOOK_SECRET=<Clerk webhook signing secret>
```

The Drizzle configuration loads `.env`; make `DATABASE_URL` available there or in the shell before running migrations:

```bash
npx drizzle-kit generate
npx drizzle-kit push
```

Start the development server:

```bash
npm run dev
```
