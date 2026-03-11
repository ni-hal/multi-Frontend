# Multi Frontend - E-Commerce Platform

A modern, full-featured e-commerce platform built with Next.js 15, featuring digital card sales, wallet management, referral system, and comprehensive user profiles.

## 🚀 Quick Start

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

## 📋 Tech Stack

- **Framework:** Next.js 15 (App Router)
- **UI Library:** React 19
- **Language:** TypeScript 5.7
- **Styling:** Tailwind CSS 3.4
- **UI Components:** shadcn/ui, Material-UI
- **State Management:** Redux Toolkit, Redux Persist
- **Animations:** Framer Motion
- **Forms:** Formik + Yup
- **HTTP Client:** Axios
- **Authentication:** JWT, Google OAuth
- **Maps:** Leaflet, React Leaflet
- **Icons:** Lucide React, React Icons
- **Notifications:** React Hot Toast
- **Carousel:** React Slick

## 🏗️ Project Structure

```
src/
├── app/                      # Next.js App Router pages
│   ├── api/                 # API routes
│   │   ├── banner/
│   │   ├── download-invoice/
│   │   └── segments/
│   ├── e-card/              # E-card marketplace
│   │   ├── checkout/
│   │   ├── product/
│   │   └── PaymentState/
│   ├── profile/             # User profile & settings
│   │   ├── order/
│   │   ├── transaction/
│   │   ├── wallet/
│   │   └── settings/
│   ├── referral/            # Referral system
│   ├── scratch/             # Scratch card rewards
│   ├── login/               # Authentication
│   ├── signup/
│   ├── forgot-pass/
│   └── manage-address/      # Address management
├── components/
│   ├── desktop/             # Desktop-specific components
│   ├── mobile/              # Mobile-specific components
│   ├── ui/                  # Reusable UI components
│   ├── ecard/               # E-card components
│   ├── scratch/             # Scratch card components
│   └── helpers/             # Validation helpers
├── services/                # API services
│   ├── auth/
│   ├── ecardApi/
│   ├── comonApi/
│   └── AxiosConfig.ts
├── hooks/                   # Custom React hooks
│   ├── useEcardData.ts
│   ├── useLocation.ts
│   └── useSegmentHandler.ts
├── lib/                     # Utilities
│   ├── store.ts            # Redux store
│   ├── auth-utils.ts
│   ├── token-utils.ts
│   └── validations.ts
└── public/
    └── assets/              # Static assets
        ├── auth/
        ├── product/
        ├── landingPage/
        └── segments/
```

## ✨ Features

### 🛍️ E-Commerce
- Digital card marketplace with categories
- Product browsing with filters
- Shopping cart & checkout
- Add-on products
- Order tracking & history
- Invoice download

### 👤 User Management
- Email/password authentication
- Google OAuth integration
- Profile management
- Address management with geolocation
- Phone number validation

### 💰 Wallet & Payments
- Digital wallet system
- Transaction history
- Multiple payment methods
- Payment state tracking

### 🎁 Rewards & Referrals
- Scratch card rewards system
- Referral program
- Referral history tracking
- Reward notifications

### 📱 Responsive Design
- Mobile-first approach
- Separate mobile/desktop components
- Touch-optimized interactions
- Progressive Web App ready

### 🔔 Notifications
- Real-time notifications
- Toast notifications
- Push notification support

### 🗺️ Location Services
- Interactive maps (Leaflet)
- Geolocation support
- Address autocomplete
- Location-based services

## 🔧 Configuration

### Environment Variables

Create a `.env.local` file:

```env
NEXT_PUBLIC_GOOGLE_MAPS_API_KEY=your_google_maps_key
NEXT_PUBLIC_API_URL=your_api_url
NEXT_PUBLIC_GOOGLE_CLIENT_ID=your_google_oauth_client_id
```

### Next.js Config

The project includes:
- Geolocation permissions
- Custom headers
- File tracing for deployment

## 📜 Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm start        # Start production server (port 1025)
npm run lint     # Run ESLint
```

## 🎨 UI Components

Built with shadcn/ui:
- Button
- Card
- Skeleton loaders
- Dialog
- Dropdown menu

Custom components:
- Loading skeletons
- YouTube skeleton
- Location modals
- Payment modals

## 🔐 Authentication

- JWT token management
- Secure token storage
- Protected routes
- Session persistence
- OAuth integration

## 🌐 API Integration

Centralized API management:
- Axios interceptors
- Token refresh logic
- Error handling
- Request/response transformation

## 📦 State Management

Redux Toolkit with:
- Auth slice
- Persistent storage
- Type-safe actions
- Async thunks

## 🎯 Key Pages

- `/` - Landing page
- `/e-card` - E-card marketplace
- `/e-card/product` - Product details
- `/e-card/checkout` - Checkout flow
- `/profile` - User profile
- `/profile/wallet` - Wallet management
- `/profile/order/history` - Order history
- `/profile/transaction/history` - Transaction history
- `/referral` - Referral program
- `/scratch` - Scratch cards
- `/manage-address` - Address management
- `/notification` - Notifications

## 🚢 Deployment

### Docker

```bash
docker build -t multifrontend .
docker run -p 1025:1025 multifrontend
```

### Vercel/Netlify

```bash
npm run build
```

Deploy the `.next` folder

## 🔒 Security

- HTTPS enforced
- JWT token encryption
- XSS protection
- CSRF protection
- Secure cookie handling
- Input validation (Yup)

## 📱 Mobile Features

- Touch gestures
- Mobile-optimized layouts
- Bottom navigation
- Swipe actions
- Mobile payment integration

## 🎨 Styling

- Tailwind CSS utility classes
- Custom CSS modules
- Responsive breakpoints
- Dark mode ready
- Animation utilities

## 🧪 Best Practices

- TypeScript strict mode
- Component composition
- Custom hooks
- Error boundaries
- Code splitting
- Lazy loading
- SEO optimization

## 📄 License

MIT

## 🤝 Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Open pull request

## 📞 Support

For issues and questions, please open a GitHub issue.
