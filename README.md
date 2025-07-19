# Slide-AI

[Live Demo](https://automation-master-seventh.vercel.app/)

Slide-AI revolutionizes how you connect with your audience on Instagram. Automate responses and boost engagement effortlessly, turning interactions into valuable business opportunities.

## Features

- **Instagram Automation:** Automate replies to comments and direct messages on Instagram.
- **AI-Powered Responses:** Generate smart, context-aware replies using AI (premium plan).
- **Analytics & Insights:** Track engagement and automation performance.
- **Integrations:** Connect your Instagram account securely.
- **Subscription Plans:** Free and premium plans with Stripe-powered billing.
- **User Dashboard:** Manage automations, integrations, and account settings.
- **Modern UI:** Built with Next.js, Tailwind CSS, and Radix UI components.

## Plans

### Free Plan ($0/month)
- Boost engagement with target responses
- Automate comment replies to enhance audience interaction
- Turn followers into customers with targeted messaging

### Smart AI Plan ($99/month)
- All features from Free Plan
- AI-powered response generation
- Advanced analytics and insights
- Priority customer support
- Customer branding options

## Tech Stack

- **Frontend:** Next.js (App Router, React, TypeScript)
- **Styling:** Tailwind CSS, Radix UI
- **State Management:** Redux Toolkit, React Query
- **Authentication:** Clerk
- **Database:** PostgreSQL (via Prisma ORM)
- **Payments:** Stripe
- **AI Integration:** OpenAI API
- **Other:** Axios, Lucide React Icons

## Getting Started

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd slide-ai
```

### 2. Install dependencies

```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

### 3. Set up environment variables

Create a `.env` file in the root directory and add the following (replace with your actual keys):

```
DATABASE_URL=postgresql://<user>:<password>@<host>:<port>/<db>
STRIPE_SECRET_KEY=sk_test_...
CLERK_SECRET_KEY=...
OPEN_AI_KEY=...
```

### 4. Run database migrations

```bash
npx prisma migrate deploy
```

### 5. Start the development server

```bash
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000) to view the app.

## Project Structure

- `src/app/` - Next.js app directory (routing, pages, layouts)
- `src/components/` - UI and global components
- `src/actions/` - Server actions for automations, integrations, user, and webhooks
- `src/constants/` - Static configuration (plans, menu, etc.)
- `src/hooks/` - Custom React hooks
- `src/lib/` - Utility libraries (Prisma, Stripe, OpenAI, etc.)
- `src/redux/` - Redux slices and store
- `prisma/` - Prisma schema and migrations

## License

[MIT](LICENSE)
