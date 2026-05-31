<p align="center">
  <img src="https://img.shields.io/badge/Next.js-14_App_Router-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-100%25-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Prisma-ORM-2D3748?style=for-the-badge&logo=prisma&logoColor=white" />
  <img src="https://img.shields.io/badge/Stripe-Payments-635BFF?style=for-the-badge&logo=stripe&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
</p>

<h1 align="center">🐍 CaseCobra — Full-Stack Custom Phone Case Store</h1>

<p align="center">
  A production-ready, full-stack e-commerce platform for ordering custom phone cases. Built end-to-end with Next.js 14 App Router, TypeScript, PostgreSQL (Prisma), Stripe payments, and Kinde authentication.
</p>

<p align="center">
  <a href="https://github.com/AliMoradpour/caseCobra-next-e-commerce-">View Repo</a> · <a href="https://alimoradpour.vercel.app">Portfolio</a>
</p>

---

## ✨ Features

- 🛠️ **Complete e-commerce shop** built from scratch with Next.js 14
- 🎨 **Custom phone-case configurator** — drag-and-drop image uploads with `react-rnd` & `react-dropzone`
- 🔑 **Authentication** via Kinde Auth (social + email login)
- 💳 **Stripe payments** — full checkout flow with webhook handling
- 🗄️ **PostgreSQL database** managed with Prisma ORM
- 📊 **Secret admin dashboard** to manage and track orders
- ✉️ **Transactional emails** via Resend — thank-you emails after purchase (`@react-email/components`)
- 🌟 **Apple-inspired UI** built with shadcn/ui and Radix primitives
- 📤 **File uploads** via UploadThing
- 🎊 **Confetti animation** on order success (`react-dom-confetti`)
- ⌨️ **100% TypeScript** — zero `any` types, strict type safety throughout

---

## 🛠️ Tech Stack

| Layer          | Technology                                      |
|----------------|--------------------------------------------------|
| Framework      | Next.js 14 (App Router)                          |
| Language       | TypeScript                                       |
| Styling        | Tailwind CSS · shadcn/ui · Radix UI              |
| Animations     | Framer Motion                                    |
| Auth           | Kinde Auth                                       |
| Payments       | Stripe + Webhooks                                |
| Database       | PostgreSQL via Prisma ORM                        |
| File Uploads   | UploadThing                                      |
| Email          | Resend + React Email                             |
| Validation     | Zod                                              |
| State          | Tanstack Query v5                                |
| Notifications  | Sonner                                           |

---

## 🚀 Getting Started

### Prerequisites

- Node.js ≥ 18
- PostgreSQL database (local or hosted, e.g. Neon / Supabase)
- Stripe account
- Kinde account
- UploadThing account

### Installation

```bash
git clone https://github.com/AliMoradpour/caseCobra-next-e-commerce-.git
cd caseCobra-next-e-commerce-
npm install
```

### Environment Variables

Create a `.env` file in the root:

```env
# Database
DATABASE_URL=postgresql://...

# Kinde Auth
KINDE_CLIENT_ID=
KINDE_CLIENT_SECRET=
KINDE_ISSUER_URL=
KINDE_SITE_URL=http://localhost:3000
KINDE_POST_LOGOUT_REDIRECT_URL=http://localhost:3000
KINDE_POST_LOGIN_REDIRECT_URL=http://localhost:3000/auth-callback

# Stripe
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=

# UploadThing
UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=

# Resend
RESEND_API_KEY=

# Admin
ADMIN_EMAIL=your@email.com
```

### Database Setup

```bash
npx prisma generate
npx prisma db push
```

### Run Dev Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

---

## 📁 Project Structure

```
caseCobra-next-e-commerce-/
├── prisma/
│   └── schema.prisma       # Database schema
├── src/
│   ├── app/                # Next.js App Router (pages, layouts, API routes)
│   ├── components/         # Reusable UI components
│   ├── lib/                # Utilities, Stripe, Prisma client
│   └── validators/         # Zod schemas
├── public/                 # Static assets
└── tailwind.config.ts
```

---

## 📸 Screenshots

> _Add screenshots of the configurator, checkout flow, and admin dashboard._

---

## 🤝 Author

**Ali Moradpour** — [alimoradpour.vercel.app](https://alimoradpour.vercel.app) · [GitHub](https://github.com/AliMoradpour) · [LinkedIn](https://linkedin.com/in/ali-moradpour-04976316a)
