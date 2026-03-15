This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

### Prerequisites
1. **Database:** This project uses Prisma with PostgreSQL for production. You need a hosted PostgreSQL database (e.g., [Vercel Postgres](https://vercel.com/docs/storage/vercel-postgres), [Supabase](https://supabase.com/), or [Neon](https://neon.tech/)).
2. **Environment Variables:** You must set the following in your Vercel project settings:
   - `DATABASE_URL`: Your production PostgreSQL connection string.
   - `JWT_SECRET`: A random string for token security.

### Steps
1. Push your code to a GitHub/GitLab/Bitbucket repository.
2. Import the project into [Vercel](https://vercel.com/new).
3. Vercel will automatically detect Next.js and use the `pnpm` environment.
4. Add your Environment Variables in the "Environment Variables" section during import.
5. Click **Deploy**.

The build command (`prisma generate && next build`) ensures that the Prisma client is generated before building the Next.js application.

