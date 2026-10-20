# Smart-Price-Tracker
A web application that tracks product prices across online shopping platforms, monitors price changes, and helps users find the best deals. Built to simplify price comparison and make smarter shopping decisions.
project strcture-
dealdrop/
├── app/
│   ├── page.js                         # Landing page with product input
│   ├── actions.js                      # Server actions for DB operations
│   ├── auth/
│   │   └── callback/
│   │       └── route.js                # OAuth callback handler
│   └── api/
│       └── cron/
│           └── check-prices/
│               └── route.js            # Cron endpoint for price checks
├── components/
│   ├── ui/                             # shadcn/ui components
│   ├── AddProductForm.js               # Product URL input with auth modal
│   ├── ProductCard.js                  # Product display with chart toggle
│   ├── PriceChart.js                   # Recharts price history
│   └── AuthModal.js                    # Google sign-in modal
├── lib/
│   ├── firecrawl.js                    # Firecrawl API integration
│   ├── email.js                        # Resend email templates
│   └── utils.js                        # Utility functions
├── utils/
│   └── supabase/
│       ├── client.js                   # Browser Supabase client
│       ├── server.js                   # Server Supabase client
│       └── middleware.js               # Session refresh middleware
├── supabase/
│   └── migrations/
│       ├── 001_schema.sql              # Database tables & RLS
│       └── 002_setup_cron.sql          # Cron job setup
├── proxy.ts                            # Next.js 15 proxy (replaces middleware)
└── .env.local                          # Environment variables
