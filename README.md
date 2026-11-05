# Demo Invoice App Starter

A full-stack Next.js invoicing app with Clerk authentication and per-user invoices stored in Neon Postgres through Drizzle.

## Getting Started

- Set up a new project

```bash
npx create-next-app my-invoicing -e https://github.com/colbyfayock/demo-invoicing-starter
```

- Navigate to your new project

```bash
cd my-invoicing
```

- Install dependencies

```bash
npm install
```

- Configure Clerk and Neon credentials in `.env.local` (`NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`, `CLERK_SECRET_KEY`, and `DATABASE_URL`; `CLERK_WEBHOOK_SECRET` is optional for the Clerk webhook endpoint). Then run the database migrations:

```bash
npx drizzle-kit generate
npx drizzle-kit push
```

- Start the development server

```bash
npm run dev
```
