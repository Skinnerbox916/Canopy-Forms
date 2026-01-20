# Can-O-Forms

A self-hosted forms backend with minimal admin UI for static sites.

## What is this?

Can-O-Forms is a lightweight, self-hosted alternative to services like Formspree or Google Forms. It provides:

- **Public submission API** for static sites (Astro, Figma Sites, etc.)
- **Admin UI** to manage sites, forms, and submissions
- **Email notifications** for new submissions
- **Spam protection** via honeypot fields and rate limiting
- **Multi-tenant architecture** supporting multiple sites per user

Perfect for personal sites and client projects where you want full control over form data without relying on third-party services.

## Project Status

🚧 **Early Development** – The project scaffold is in place, but core features are not yet implemented. See [PRD.md](./PRD.md) for the complete requirements specification.

## Architecture

- **Framework**: Next.js (App Router)
- **Database**: PostgreSQL with Prisma ORM
- **Auth**: NextAuth (credentials only)
- **Email**: Nodemailer (Migadu SMTP)
- **Deployment**: Designed for Coolify self-hosting

## Getting Started

### Prerequisites

- Node.js 20+
- PostgreSQL database

### Local Development

```bash
# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your database credentials

# Run database migrations
npm run db:migrate

# Seed initial admin user
npm run db:seed

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see the app.

## Documentation

- [PRD.md](./PRD.md) – Complete product requirements
- API documentation – Coming soon
- Deployment guide – Coming soon

## License

See [LICENSE](./LICENSE) file for details.
