# eChef Mobile App

A React Native mobile application for discovering and booking talented chefs. Built with Expo, TypeScript, Clerk authentication, Appwrite backend, and Stripe payments.

## Features

- **TikTok-Style Video Feed**: Discover chefs through engaging cooking videos
- **Location-Based Discovery**: Find chefs nearby with geolocation
- **Booking System**: Easy booking with transparent pricing
- **Review & Rating System**: Multi-category ratings with photo uploads
- **Subscription System**: Multiple tiers with exclusive content and benefits
- **Event System**: Cooking classes, workshops, and culinary experiences
- **Chef Dashboard**: Manage bookings, videos, and earnings
- **Secure Payments**: Stripe integration for payments and subscriptions

## Tech Stack

- **Frontend**: React Native, Expo, TypeScript
- **Styling**: NativeWind (Tailwind CSS for React Native)
- **Authentication**: Clerk
- **Backend**: Appwrite (Database, Storage, Functions)
- **Payments**: Stripe
- **Navigation**: Expo Router

## Getting Started

### Prerequisites

- Node.js 18+
- Expo CLI
- iOS Simulator or Android Emulator (or physical device)

### Installation

1. Clone the repository
2. Install dependencies:
   \`\`\`bash
   npm install
   \`\`\`

3. Copy `.env.example` to `.env` and fill in your environment variables

4. Start the development server:
   \`\`\`bash
   npm start
   \`\`\`

5. Run on your preferred platform:
   \`\`\`bash
   npm run ios     # iOS
   npm run android # Android
   \`\`\`

## Environment Variables

See `.env.example` for required environment variables:

- Clerk authentication keys
- Appwrite endpoint and project configuration
- Appwrite collection IDs
- Stripe publishable key

## Project Structure

\`\`\`
app/
  (auth)/          # Authentication screens
  (tabs)/          # Main tab navigation
  booking/         # Booking details and management
  chef/            # Chef profile and dashboard
  events/          # Event browsing and registration
  review/          # Review creation
  subscriptions/   # Subscription management
  exclusive-content/ # Premium content
components/        # Reusable components
hooks/            # Custom React hooks
lib/              # Utilities and configurations
scripts/          # Database setup scripts
\`\`\`

## Key Features Implementation

### Authentication Flow
- Clerk-based authentication with email/password
- Automatic user profile creation in Appwrite
- Secure token storage with Expo SecureStore

### Review System
- Multi-category ratings (food, service, presentation, value)
- Photo uploads with reviews
- Verified booking reviews only
- Chef rating aggregation

### Subscription System
- Multiple subscription tiers (Basic, Premium, VIP)
- Exclusive content access
- Priority booking for subscribers
- Discount benefits
- Stripe subscription management

### Event System
- Cooking classes and workshops
- Virtual and in-person events
- Group bookings with capacity management
- Waitlist functionality
- Event-specific reviews

## Database Schema

The app uses Appwrite with the following collections:

- Users
- Chefs
- Services
- Bookings
- Reviews
- Videos
- Video Likes
- Subscription Plans
- User Subscriptions
- Exclusive Content
- Subscription Transactions
- Event Templates
- Event Schedules
- Event Attendees
- Event Waitlist
- Event Reviews

## Contributing

This is a hackathon project. Feel free to fork and modify for your own use.

## License

MIT
# echef
