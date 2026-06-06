# Health Lab Tracker V2

A modern health lab report tracking application with complete authentication flow, built with React and Tailwind CSS, featuring a purple (#b3a8ff) and lime green (#d4e95e) theme.

## Features

### Authentication Pages
- **Landing Page**: Animated welcome screen with floating shapes
- **Sign In with Email**: Email and password authentication with "Forgot password?" link
- **Sign In with Phone**: Phone number authentication with country code selector
- **Create Account**: Full registration form with password confirmation
- **Social Sign In**: Google authentication option

### Health Tracking Pages
- **Home Page**: Health score card with progress rings, key parameters grid, cholesterol trends chart, and AI-powered health insights
- **Reports Page**: Lab reports grouped by month with score circles and status badges
- **Trends Page**: Parameter cards with expandable charts and informational popups
- **Upload Page**: Three upload options with helpful tips
- **Profile Page**: User statistics and settings management
- **Health Score Detail**: Detailed breakdown showing calculation methodology

## Design System

All pages follow a consistent design pattern:
- **Purple rounded headers** (#b3a8ff with rounded-b-[48px])
- **White rounded cards** (rounded-[32px]) with subtle shadows
- **Light gray backgrounds** (#f1f2f4)
- **Dark action buttons** (#1c1b1b)
- **Purple accents** (#9EA4F5) for links and secondary actions
- **Lime green highlights** (#d4e95e) for primary CTAs
- **Glassmorphism bottom navigation bar**
- **Smooth animations** and transitions throughout

## Tech Stack

- React 18.3
- Tailwind CSS 4.1
- Vite 6.3
- TypeScript
- Lucide React (icons)
- Recharts (data visualization)
- Motion (animations)

## Getting Started

```bash
# Install dependencies
pnpm install

# Start development server
pnpm run dev

# Build for production
pnpm run build
```

## Project Structure

```
src/
├── app/
│   ├── components/
│   │   ├── SignIn.tsx           # Landing page with navigation
│   │   ├── SignInEmail.tsx      # Email/password sign in
│   │   ├── SignInPhone.tsx      # Phone number sign in
│   │   ├── CreateAccount.tsx    # Registration form
│   │   ├── Reports.tsx          # Lab reports list
│   │   ├── Trends.tsx           # Parameter trends
│   │   ├── Upload.tsx           # Upload interface
│   │   ├── Profile.tsx          # User profile
│   │   ├── AskAI.tsx            # AI chat interface
│   │   ├── HealthScore.tsx      # Score breakdown
│   │   └── ui/                  # Radix UI components
│   └── App.tsx                  # Main app with navigation
├── styles/
│   ├── theme.css                # Design tokens
│   ├── fonts.css                # Font imports
│   ├── globals.css              # Global styles & animations
│   └── tailwind.css             # Tailwind config
└── imports/                     # Images and assets
```

## Authentication Flow

1. **Landing Page** → Choose sign in method
2. **Sign In with Email** → Enter credentials or use social/phone options
3. **Sign In with Phone** → Enter phone number with country code
4. **Create Account** → Register with name, email, and password
5. **Main App** → Access all health tracking features

## Animations

- **Float**: Gentle floating motion for decorative shapes
- **Fade In**: Smooth content appearance
- **Pulse**: Attention-drawing glow effect on primary CTAs
- **Hover Effects**: Interactive button states

## Color Palette

- Primary Purple: `#b3a8ff`
- Accent Purple: `#9EA4F5`
- Lime Green: `#d4e95e`
- Dark Text: `#1c1b1b`
- Light Background: `#f1f2f4`
- Card Background: `#f8f8fc`

## License

MIT
