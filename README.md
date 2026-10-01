# Bipul Adhikari — Premium Personal Portfolio & WebCraft Studios Ecosystem

A modern, high-performance personal portfolio and digital brand platform for **Bipul Adhikari** — Programmer, Graphic Designer, Software Developer, Entrepreneur, and Founder & CEO of **WebCraft Studios Pvt. Ltd.**

Built as a production-grade digital product combining **code craftsmanship, editorial design aesthetics, and business scalability**.

---

## 🌟 Architecture Overview

The project is structured with a decoupled **`frontend/`** and **`backend/`** architecture:

```
bipul-adhikari-portfolio/
├── frontend/                  # Next.js 16 (App Router) + TypeScript + Tailwind CSS 4 + Framer Motion
│   ├── app/
│   │   ├── layout.tsx         # Space Grotesk + Inter fonts, JSON-LD Schema (Person, Org, WebSite)
│   │   ├── page.tsx           # Page 1: Home (Hero, interactive code terminal, marquee, work, services)
│   │   ├── about/             # Page 2: About / Profile (Story, journey timeline, 7-step approach, skills)
│   │   ├── projects/          # Projects Gallery with category filters and rich case studies
│   │   ├── services/          # Detailed breakdown of all 8 core services & WebCraft Studios agency
│   │   ├── contact/           # Working inquiry form with validation and honeypot protection
│   │   ├── not-found.tsx      # Custom 404 page with terminal diagnostic UI
│   │   ├── robots.ts          # Automated robots.txt
│   │   ├── sitemap.ts         # Automated sitemap.xml
│   │   └── globals.css        # Void Black & Electric Blue design system, custom scrollbars, animations
│   ├── components/            # Modular UI components, layouts, and interactive sections
│   └── lib/data/              # Single source of truth data (profile, projects, skills, services, timeline)
│
├── backend/                   # Node.js + Express + TypeScript API Service
│   ├── src/
│   │   ├── index.ts           # Server entry point with Helmet, CORS, and request logging
│   │   ├── routes/            # /api/health, /api/contact, /api/projects, /api/services
│   │   ├── middleware/        # Rate limiting and Zod request validation
│   │   └── storage/           # In-memory and persistent JSON storage (modular for Supabase/PostgreSQL)
│   └── tsconfig.json
└── README.md
```

---

## 🚀 Quick Start Guide

### Prerequisites
- **Node.js**: v18+ (tested on Node v24)
- **NPM**: v9+ (tested on NPM v11)

---

### 1. Running the Backend API Server

```bash
cd backend
npm install
npm run dev
```

The API server will start on `http://localhost:5000`.

Key endpoints:
- **`GET /api/health`**: Health check and server uptime
- **`POST /api/contact`**: Submit inquiry (includes Zod validation, rate limiter, and bot honeypot protection)
- **`GET /api/projects`**: Structured project portfolio dataset
- **`GET /api/services`**: Structured services dataset

To build for production:
```bash
npm run build
npm start
```

---

### 2. Running the Frontend Application

In a separate terminal:

```bash
cd frontend
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

To create an optimized production build:
```bash
npm run build
npm start
```

---

## 🎨 Design System & Palette

- **Primary Background**: `#08090B` (Void Black)
- **Secondary Surface**: `#111318` (Dark Graphite)
- **Card / Panel Background**: `#0F1218`
- **Primary Accent**: `#3B82F6` (Electric Blue)
- **Accent Highlight**: `#60A5FA` (Sky Blue)
- **Typography**:
  - Headings: `Space Grotesk` (editorial & modern tech feel)
  - Body & UI: `Inter` (optimal legibility across all viewport sizes)
- **Visual Features**:
  - Interactive live code terminal with multi-tab snippets
  - Subtle mouse spotlight glow on desktop (disabled on touch devices)
  - Continuous animated skills ticker with `prefers-reduced-motion` compliance
  - 01–08 interactive services list with real-time hover disclosures
  - Visual 7-step methodology: `Discover → Plan → Design → Build → Test → Launch → Improve`

---

## 🔒 Security & Performance Features

1. **Input Validation**: Strict Zod schema validation on both client and server.
2. **Anti-Spam Protection**: Invisible honeypot field (`_hp_company`) traps malicious web bots without requiring frustrating user CAPTCHAs.
3. **Rate Limiting**: Configured with `express-rate-limit` to prevent automated endpoint abuse.
4. **Technical SEO**:
   - Semantic HTML5 structure
   - Dynamic `robots.txt` and `sitemap.xml`
   - Schema.org JSON-LD tags (`Person`, `Organization` for WebCraft Studios, `WebSite`)
   - Complete OpenGraph and Twitter card metadata
5. **Accessibility**: Visible keyboard focus rings (`focus-visible:ring-2 focus-visible:ring-blue-500`), semantic tags, ARIA labels, and color contrast adherence.

---

## 💼 WebCraft Studios Pvt. Ltd. Integration

The portfolio seamlessly highlights Bipul Adhikari's role as **Founder & CEO** of **WebCraft Studios Pvt. Ltd.** with:
- Dedicated agency spotlight section: *"We Craft Ideas Into Reality."*
- Full showcase of enterprise services (Cloud solutions, AI automation, custom software, SaaS MVPs).
- Direct callouts for client retainers and enterprise partnerships.

---

## 📄 License & Attribution

Designed & built for **Bipul Adhikari** and **WebCraft Studios Pvt. Ltd.** All rights reserved.
