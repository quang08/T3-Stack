# Chirp

Full-stack app built with [T3 Stack](https://create.t3.gg/)

- **Framework**: [Next.js](https://nextjs.org/)
- **Database**: [PlanetScale](https://planetscale.com/)
- **Type-safety**: [tRPC](https://trpc.io/)
- **ORM**: [Prisma](https://prisma.io/)
- **Authentication**: [Clerk](https://clerk.com/)
- **Deployment**: [Vercel](https://vercel.com)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Rate Limit**: [Upstash](https://upstash.com/)

## Home (Pre-signed in)
<img width="508" alt="preSignin" src="https://user-images.githubusercontent.com/84165564/230702532-8e30e22a-e7d4-42f9-874d-c930d0fce0d8.png">

## Clerk Sign in
<img width="508" alt="clerkSigninPage" src="https://user-images.githubusercontent.com/84165564/230702531-1efb307c-f868-491d-896c-97240800867f.png">

## Home (Signed in)
<img width="508" alt="signedIn" src="https://user-images.githubusercontent.com/84165564/230702529-ec074bcd-c286-4d57-86af-c95198740be2.png">

## Loading state
- hydrate the input, only the feed would have a loading state
<img width="508" alt="loading" src="https://user-images.githubusercontent.com/84165564/230702527-0aa97ed7-3d35-4470-b896-4698fe4c5411.png">

## Input validation
<img width="508" alt="invalidInput" src="https://user-images.githubusercontent.com/84165564/230702525-a18bef4c-b1f2-43d8-977d-11b1cf534604.png">

## Profile View
<img width="508" alt="profilePage" src="https://user-images.githubusercontent.com/84165564/230702522-efc06e59-4914-46e0-88d9-208d613f5058.png">

## Post View
<img width="508" alt="postView" src="https://user-images.githubusercontent.com/84165564/230702519-04f36988-81c4-4145-a37a-2b280b4a2a91.png">

## Environment Variables

To run this project, you will need to add the following environment variables to your `.env` file

```bash
# Database URL for Prisma
DATABASE_URL="mysql://johndoe:randompassword@localhost:5432/mydb?schema=public"

# Clerk for auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

# Upstash for rate limiting
UPSTASH_REDIS_REST_URL=""
UPSTASH_REDIS_REST_TOKEN=""
```


## Run Locally

Clone the project

```bash
  git clone https://github.com/quang08/T3-Stack
```

Go to the project directory

```bash
  cd T3-Stack
```

Install dependencies

```bash
  npm install
```

Apply migrations to database

```bash
  npm migrate-dev
```

Seed the database

```bash
  npm db-seed
```

Start the server

```bash
  npm run dev
```
