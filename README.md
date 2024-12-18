This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Banking website

This is an all in one banking website. Where users can connect all their different bank accounts, get an overview of their spending habits, and transfer funds between accounts.

## Deployed website

You can view this website at [`Vercel`](https://banking-neon-kappa.vercel.app/)

The website is running using a sandbox environment, so you can sign up with fake details but make sure you use a US address.
To add or connect a bank account you'll need to use the Plaid sandbox credential as follows:

username: `app_good`
password: `pass_good`

## Running locally

Add environment variables following the `.env.example` file.
At the time of writing Dwolla, Appwrite, and Plaid all offer free tiers with no credit card details needed during sign up.

Run the development server:

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

## Technologies used

Written in

- NextJS
- Tailwind
- Typescript

Using

- Dwolla: for managing transactions between accounts, allowing users to send, receive, and request money.
- Appwrite: which is an open source backend server, handling the user auth and database.
- Plaid: to connect bank accounts to third-party applications, simplifying adding financial daata, transaction and balance updates. For this website I'm using the Plaid sandbox environment, not dealing with actual bank accounts.

- Sentry for logging
