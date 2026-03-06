# VERDA

Supply chain transparency protocol for the global food industry. Every product gets a verifiable journey from soil to shelf.

## About

VERDA is a blockchain-based food traceability platform that combines IoT sensors, blockchain verification, and QR scanning to create immutable records of every product's journey from farm to shelf.

### The Problem We Solve

- **$40B+** annual food fraud globally
- **600M** people get sick from contaminated food yearly
- **$35B** cold chain losses annually
- Traditional recalls take 2-3 weeks and destroy entire batches

### Our Solution

- **QR Journey Viewer** - Consumer scans, full journey in 2 seconds. No app required.
- **Cold Chain Monitoring** - Real-time IoT sensors track temperature and humidity.
- **Smart Recall System** - Surgical precision recalls in hours, not weeks.
- **Blockchain Verification** - Immutable, tamper-proof records.

## Tech Stack

| Technology | Purpose |
|------------|---------|
| Astro 5 | Static site generator |
| TailwindCSS 4 | Styling framework |
| Lucide Icons | Icon library |
| TypeScript | Type checking |

### Backend (Platform)

| Technology | Purpose |
|------------|---------|
| Go + Rust | Backend services |
| TimescaleDB | Time-series database |
| Kafka | Event streaming |
| LoRaWAN | IoT network |

## Project Structure

```
VERDA/
├── src/
│   ├── pages/              # Page routes
│   │   ├── index.astro     # Home page
│   │   ├── about.astro     # About page
│   │   ├── product.astro   # Product overview
│   │   ├── technology.astro# Technology overview
│   │   ├── docs.astro      # Developer docs
│   │   ├── demo/           # Interactive demos
│   │   ├── product/        # Product deep-dives
│   │   └── technology/     # Tech deep-dives
│   ├── components/         # Reusable components
│   │   ├── layout/         # Navbar, Footer
│   │   ├── cards/          # Card components
│   │   ├── shared/         # Base UI components
│   │   └── decorative/     # Visual elements
│   ├── layouts/            # Page layouts
│   │   └── BaseLayout.astro
│   └── styles/
│       └── global.css      # Global styles & theme
├── public/                 # Static assets
├── astro.config.mjs        # Astro configuration
├── tsconfig.json           # TypeScript config
└── package.json            # Dependencies
```

## Getting Started

### Prerequisites

- Node.js >= 18.20.8
- pnpm (recommended)

### Installation

```bash
# Clone the repository
git clone https://github.com/verda-protocol/verda.git
cd verda

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

The site will be available at `http://localhost:4321`

## Commands

| Command | Action |
|---------|--------|
| `pnpm install` | Install dependencies |
| `pnpm dev` | Start dev server at `localhost:4321` |
| `pnpm build` | Build production site to `./dist/` |
| `pnpm preview` | Preview production build locally |

## Features

### Pages

- **Home** - Landing page with hero, features, roadmap
- **About** - Company story, team, mission, values
- **Product** - Product suite overview (QR viewer, cold chain, recall)
- **Technology** - Architecture and security deep-dives
- **Demo** - Interactive product demonstrations
- **Docs** - Developer documentation and API reference

### Design System

- Custom green/earth-tone color palette
- Fraunces display font
- Responsive mobile-first design
- Scroll reveal animations
- 3D card effects
- Dark mode ready components

## Deployment

### Deploy to Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/verda-protocol/verda)

#### Option 1: One-Click Deploy

1. Click the "Deploy with Vercel" button above
2. Connect your GitHub account
3. Configure project settings (optional)
4. Deploy

#### Option 2: Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Login to Vercel
vercel login

# Deploy to preview
vercel

# Deploy to production
vercel --prod
```

#### Option 3: Git Integration

1. Push your code to GitHub/GitLab/Bitbucket
2. Import project at [vercel.com/new](https://vercel.com/new)
3. Vercel auto-detects Astro and configures build settings
4. Deploy

### Environment Variables

No environment variables required for the static site.

### Build Output

- **Output Directory:** `dist`
- **Build Command:** `pnpm build`
- **Install Command:** `pnpm install`

## Roadmap

1. **Phase 1** - Single chain pilot with 100 products
2. **Phase 2** - Multi-brand expansion to 10K products
3. **Phase 3** - Industry platform serving 100+ brands
4. **Phase 4** - Open protocol across 20+ countries

## Team

- **Sarah Chen** - CEO & Co-founder (ex-Nestlé, MIT MBA)
- **Adi Pratama** - CTO & Co-founder (ex-Google, Blockchain contributor)
- **Dr. Maria Santos** - Chief Science Officer (WHO consultant)
- **James Okonkwo** - Head of Engineering (IoT/Rust specialist)

## Contact

- Email: hello@verda.so
- Twitter: [@verda_protocol](https://twitter.com/verda_protocol)
- GitHub: [verda-protocol](https://github.com/verda-protocol)
- LinkedIn: [Verda](https://linkedin.com/company/verda)

## License

Copyright 2026 Verda Protocol. All rights reserved.
