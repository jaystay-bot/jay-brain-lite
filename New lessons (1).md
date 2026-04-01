# lessons.md — Core Permanent Lessons

## App Router
- Use Next.js App Router only
- Use TypeScript only
- Use shadcn/ui and Lucide React for UI defaults

## Supabase
- Enable RLS on every table
- Use server-side Supabase access where appropriate
- Do not expose service-role credentials to the client

## Stripe
- Secret key server-side only
- Stripe webhook route lives at `app/api/webhooks/stripe/route.ts`
- Prefer Stripe Checkout unless explicitly told otherwise

## Clerk
- Wrap root layout with ClerkProvider
- Use server-side auth helpers on the server, client hooks on the client

## Scraping and APIs
- Check official API access before building scrapers
- Do not assume direct fetch works on major retailers
- Research access limits before implementation

## Build Discipline
- One task at a time
- One command at a time
- Prove the touched area works before marking done
- Prefer minimal changes over architecture expansion
- Stop and re-plan when stuck