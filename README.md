# Crypto Dashboard

A modern, feature-rich cryptocurrency dashboard built with Next.js 14, TypeScript, and Tailwind CSS. Track real-time cryptocurrency prices, market trends, and global statistics with an intuitive and responsive interface.

## 🚀 Features

### Core Functionality
- **Real-time Cryptocurrency Data**: Live prices, market caps, and 24h volume tracking
- **Advanced Search**: Filter and search through 100+ cryptocurrencies
- **Detailed Coin Analysis**: Comprehensive statistics, historical data, and price charts
- **Global Market Overview**: Total market cap, 24h volume, and market dominance
- **Trending Coins**: Discover trending cryptocurrencies in real-time
- **Price Charts**: Interactive historical price charts with multiple timeframes
- **Dark/Light Mode**: Seamless theme switching with system preference detection

### Technical Features
- **Progressive Web App (PWA)**: Installable on mobile devices with offline support
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **TypeScript**: Type-safe development with full TypeScript support
- **Modern UI/UX**: Built with Radix UI components and Tailwind CSS
- **Authentication**: NextAuth.js integration with Google OAuth support
- **State Management**: Zustand for efficient client-side state management
- **API Integration**: CoinRanking API for comprehensive cryptocurrency data
- **Code Quality**: ESLint, Prettier, and Husky pre-commit hooks

## 🛠️ Tech Stack

### Frontend
- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS + CSS Modules
- **UI Components**: Radix UI + Lucide React icons
- **Charts**: Recharts for data visualization
- **State Management**: Zustand
- **Authentication**: NextAuth.js

### Development Tools
- **Package Manager**: npm
- **Code Quality**: ESLint + Prettier
- **Git Hooks**: Husky + lint-staged
- **PWA**: next-pwa
- **Loading**: nextjs-toploader
- **Notifications**: Sonner (toast notifications)

### APIs & Services
- **Crypto Data**: CoinRanking API
- **Authentication**: Google OAuth via NextAuth.js
- **News**: Crypto news integration

## 📦 Installation

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/bhanurx100/crypto-dashboard.git
   cd crypto-dashboard
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   ```bash
   cp .env.local.sample .env.local
   ```

4. **Configure Environment Variables**
   Edit `.env.local` and add your API keys:
   ```env
   # CoinRanking API
   NEXT_PUBLIC_COINGECKO_API_KEY=your_coinranking_api_key
   
   # Google OAuth (Optional)
   GOOGLE_ID=your_google_client_id
   GOOGLE_SECRET=your_google_client_secret
   NEXTAUTH_URL=http://localhost:3000
   NEXTAUTH_SECRET=your_nextauth_secret
   ```

5. **Start Development Server**
   ```bash
   npm run dev
   ```

6. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🔧 Configuration

### API Keys Setup

1. **CoinRanking API**
   - Sign up at [CoinRanking](https://coinranking.com/api)
   - Get your API key from the dashboard
   - Add it to `NEXT_PUBLIC_COINGECKO_API_KEY` in `.env.local`

2. **Google OAuth (Optional)**
   - Go to [Google Cloud Console](https://console.cloud.google.com/)
   - Create a new project or select existing one
   - Enable Google+ API
   - Create OAuth 2.0 credentials
   - Add the credentials to your environment variables

## 📱 Usage

### Main Features

1. **Dashboard Overview**
   - View global cryptocurrency market statistics
   - Track top 10 cryptocurrencies by market cap
   - Discover trending coins

2. **Cryptocurrency Explorer**
   - Browse 100+ cryptocurrencies
   - Search and filter by name
   - View detailed statistics for each coin

3. **Coin Details**
   - Comprehensive coin statistics
   - Historical price charts
   - Market analysis and trends
   - Official links and resources

4. **Theme Customization**
   - Toggle between light and dark modes
   - System preference detection
   - Persistent theme selection

## 🏗️ Project Structure

```
crypto-dashboard/
├── public/                 # Static assets and PWA files
├── src/
│   ├── app/               # Next.js App Router pages
│   │   ├── api/          # API routes
│   │   ├── coin/         # Coin-specific pages
│   │   └── explore/      # Cryptocurrency explorer
│   ├── components/        # Reusable React components
│   │   ├── dashboard/    # Dashboard components
│   │   ├── ui/           # Base UI components
│   │   └── ...           # Other feature components
│   ├── services/         # API service configurations
│   ├── store/            # State management
│   ├── lib/              # Utility functions
│   └── container/        # Layout containers
├── .husky/               # Git hooks
├── .vscode/              # VS Code settings
└── ...                   # Configuration files
```

## 🚀 Available Scripts

```bash
# Development
npm run dev          # Start development server
npm run build        # Build for production
npm run start        # Start production server

# Code Quality
npm run lint         # Run ESLint
npm run prepare      # Setup Husky hooks
```

## 🎨 Customization

### Adding New Features
1. Create components in `src/components/`
2. Add API endpoints in `src/services/`
3. Update state management in `src/store/`
4. Add routes in `src/app/`

### Styling
- Modify `tailwind.config.ts` for theme customization
- Update `src/app/globals.css` for global styles
- Use CSS Modules for component-specific styles

## 📊 API Integration

### CoinRanking API Endpoints Used
- `/coins` - List of cryptocurrencies
- `/coin/{id}` - Coin details
- `/coin/{id}/history` - Historical price data
- `/stats` - Global market statistics

### Rate Limits
- Free tier: 100 requests per day
- Consider upgrading for production use

## 🔒 Security

- Environment variables for sensitive data
- NextAuth.js for secure authentication
- API key protection
- CORS configuration
- Content Security Policy headers

## 🌐 Deployment

### Vercel (Recommended)
1. Connect your GitHub repository to Vercel
2. Add environment variables in Vercel dashboard
3. Deploy automatically on push to main branch

### Other Platforms
```bash
npm run build
npm run start
```

Ensure environment variables are properly configured in your hosting platform.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow TypeScript best practices
- Use ESLint and Prettier configurations
- Write meaningful commit messages
- Test your changes thoroughly

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [CoinRanking](https://coinranking.com/) for cryptocurrency data API
- [Next.js](https://nextjs.org/) for the React framework
- [Tailwind CSS](https://tailwindcss.com/) for styling
- [Radix UI](https://www.radix-ui.com/) for accessible components
- [Recharts](https://recharts.org/) for data visualization

## 📞 Support

If you have any questions or need support, please:
- Open an issue on GitHub
- Check the [documentation](https://github.com/bhanurx100/crypto-dashboard/wiki)
- Review existing issues and discussions

---

**Built with ❤️ by [Bhanu Prakash](https://github.com/bhanurx100)**