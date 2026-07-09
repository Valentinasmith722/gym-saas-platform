# Gym SaaS Platform 💪

> A complete white-label platform for gyms, fitness studios, and personal trainers. Manage memberships, schedule classes, process payments, track member progress, and grow your business — all from one beautiful dashboard.

## ✨ Features

### For Gym Owners
- **Membership Management**: Monthly, annual, drop-in, and custom plans
- **Class Scheduling**: Group classes, personal training, workshops
- **Payment Processing**: Integrated payments with automatic invoicing
- **Staff Management**: Trainers, front desk, managers with role-based access
- **Analytics Dashboard**: Revenue, attendance, retention, and growth metrics
- **Marketing Tools**: Email campaigns, SMS notifications, referral programs
- **Facility Management**: Equipment tracking, maintenance schedules, room booking
- **Multi-Location**: Manage multiple gym locations from one dashboard

### For Members
- **Mobile App**: iOS and Android apps for booking and tracking
- **Class Booking**: Book classes, get waitlist notifications, cancel/reschedule
- **Progress Tracking**: Workout logs, body measurements, progress photos
- **Trainer Communication**: Message trainers, share workout plans
- **Community Feed**: Social feed for members to share achievements
- **Challenges & Gamification**: Fitness challenges, leaderboards, badges
- **Nutrition Tracking**: Log meals, get macro recommendations
- **Wearable Integration**: Apple Health, Google Fit, Fitbit, Garmin

### For Trainers
- **Client Management**: Track client progress, schedules, and goals
- **Workout Builder**: Create and assign custom workout plans
- **Schedule Management**: Set availability, manage bookings
- **Progress Reports**: Generate detailed client progress reports
- **Income Tracking**: Track sessions, commissions, and tips
- **Video Library**: Upload exercise demonstration videos

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/valentinasmith722/gym-saas-platform.git
cd gym-saas-platform

# Install dependencies
npm install

# Setup database
npx prisma migrate dev

# Seed demo data
npm run seed

# Start development server
npm run dev

# Open http://localhost:3000
```

## 📊 Dashboard Preview

```
┌─────────────────────────────────────────────────────────────┐
│  GymOS v3.0 — PowerFit Gym                                  │
├─────────────────────────────────────────────────────────────┤
│  💰 Revenue: $12,450        👥 Members: 342  ↑ 5%          │
│  📅 Classes Today: 18       🏃 Check-ins: 89               │
├─────────────────────────────────────────────────────────────┤
│  Today's Schedule                                             │
│  06:00  🏋️ CrossFit        [12/20]  ✅ Active              │
│  07:00  🧘 Yoga Flow       [18/20]  ⚠️  Almost Full        │
│  08:00  🥊 Boxing          [8/15]   ✅ Active             │
│  09:00  🚴 Spin Class      [20/20]  ❌ Full               │
│  10:00  💪 Personal Train  [3/5]    ✅ Active             │
├─────────────────────────────────────────────────────────────┤
│  Member Activity                                              │
│  Sarah M.    checked in  🏋️ CrossFit  2 min ago          │
│  Mike T.     booked      🧘 Yoga Flow  5 min ago           │
│  Jessica L.  completed   💪 Leg Day     15 min ago         │
│  David K.    cancelled   🚴 Spin Class  1 hour ago         │
└─────────────────────────────────────────────────────────────┘
```

## 🛠️ Tech Stack

- **Frontend**: Next.js 14 + Tailwind CSS + shadcn/ui
- **Backend**: Next.js API Routes + tRPC
- **Database**: PostgreSQL + Prisma ORM
- **Auth**: NextAuth.js + OAuth providers
- **Payments**: Stripe (subscriptions, one-time, invoices)
- **Real-time**: Socket.io (live bookings, notifications)
- **Mobile**: React Native (iOS + Android)
- **Storage**: AWS S3 (photos, videos, documents)
- **Email**: Resend / SendGrid
- **SMS**: Twilio
- **Analytics**: PostHog
- **Search**: Algolia (class/member search)

## 📱 Mobile App

```bash
cd mobile-app
npm install
npx expo start
# Scan QR code with Expo Go app
```

## 🎯 Use Cases

- **CrossFit Boxes**: Class scheduling, WOD tracking, leaderboard
- **Yoga Studios**: Class passes, instructor profiles, meditation content
- **Personal Trainers**: Client management, workout plans, progress tracking
- **Corporate Wellness**: Employee fitness programs, challenges, reports
- **Sports Clubs**: Team management, facility booking, event registration
- **Dance Studios**: Recital management, costume tracking, parent portal
- **Martial Arts Dojos**: Belt tracking, tournament management, video library

## 🔧 Configuration

Create a `.env` file:

```env
# Database
DATABASE_URL=postgresql://user:pass@localhost/gym_saas_db

# NextAuth
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_super_secret_key

# OAuth Providers (optional)
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

# Stripe
STRIPE_SECRET_KEY=sk_test_...
STRIPE_WEBHOOK_SECRET=whsec_...
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=pk_test_...

# Email
RESEND_API_KEY=re_...

# SMS
TWILIO_ACCOUNT_SID=AC...
TWILIO_AUTH_TOKEN=...
TWILIO_PHONE_NUMBER=+1...

# Storage
AWS_ACCESS_KEY_ID=...
AWS_SECRET_ACCESS_KEY=...
AWS_REGION=us-east-1
AWS_S3_BUCKET=...

# Algolia
ALGOLIA_APP_ID=...
ALGOLIA_API_KEY=...
ALGOLIA_SEARCH_KEY=...

# PostHog Analytics
NEXT_PUBLIC_POSTHOG_KEY=...
NEXT_PUBLIC_POSTHOG_HOST=...
```

## 💳 Payment Plans

The platform supports multiple pricing models:

### Membership Plans
- **Monthly**: $49/month — Unlimited classes
- **Annual**: $499/year — Save 15%
- **Class Pass**: $15/class — Pay per visit
- **Personal Training**: $75/session — One-on-one

### Gym Owner Pricing (White-Label)
- **Starter**: $99/month — 1 location, 100 members
- **Growth**: $199/month — 3 locations, 500 members
- **Enterprise**: $499/month — Unlimited locations, unlimited members

## 📦 Core Modules

### 1. Member Management
- Profile creation and onboarding
- Membership status and history
- Check-in/check-out tracking
- Attendance analytics
- Member retention alerts

### 2. Class & Schedule
- Recurring and one-time classes
- Instructor assignments
- Room/facility booking
- Waitlist management
- Capacity limits and social distancing

### 3. Payments & Billing
- Automated recurring billing
- Invoice generation and sending
- Payment failure handling
- Refund processing
- Revenue reporting

### 4. Workout & Progress
- Exercise library (500+ exercises)
- Workout plan builder
- Progress tracking (weight, reps, time)
- Body measurements and photos
- Achievement badges

### 5. Communication
- In-app messaging
- Email campaigns
- SMS notifications
- Push notifications (mobile)
- Announcement board

### 6. Marketing & Growth
- Referral program
- Social media integration
- Review collection
- Lead capture forms
- Promotional codes

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Ways to Contribute

- 🐛 Report bugs via GitHub Issues
- 💡 Suggest features via GitHub Discussions
- 🔧 Submit pull requests
- 🎨 Design UI components and themes
- 📖 Write documentation and tutorials
- 🌍 Translate to other languages
- 📱 Test the mobile app and report issues

## ☕ Support This Project

This platform is **100% free and open source**. We built it because we believe every gym owner, trainer, and fitness professional deserves enterprise-level tools without the enterprise-level price tag.

If Gym SaaS Platform helped you grow your business, save time on admin work, or provide a better experience for your members, consider supporting its continued development:

**Solana (USDT)**: `BKjS4agVRowFGqUuWHEKZerk3dCS52V1n4NdWaeNTo8E`

Your support helps us:
- Develop iOS and Android apps
- Add AI-powered workout recommendations
- Integrate with more wearables and fitness devices
- Create video tutorials and documentation
- Build a marketplace for gym themes and plugins
- Support gym owners worldwide with better tools
- Keep the platform free for small gyms and startups

*Every contribution helps us empower fitness professionals everywhere. Thank you for being part of our mission.* 🙏

## 📄 License

MIT License — free to use, modify, and distribute.

## 🌟 Star History

If this platform helped your gym grow, please give it a star ⭐ on GitHub!

---

*Built with ❤️ for fitness professionals everywhere | 2026*
