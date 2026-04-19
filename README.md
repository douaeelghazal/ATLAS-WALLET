# ATLAS-WALLET 

A comprehensive digital wallet platform that combines AI-powered shopping assistance with secure payment management. Atlas Wallet enables users to manage their finances, discover partner offers, and make seamless purchases through an intelligent shopping assistant.

##  Features

- **AI-Powered Shopping Assistant**: Chat-based shopping assistant powered by LangChain and LLMs
- **Digital Wallet Management**: Secure wallet with balance tracking and transaction history
- **Partner Catalog**: Browse and manage partner offers and discounts
- **Order Tracking**: Real-time order status tracking and management
- **Payment Processing**: Integrated payment sheet for secure transactions
- **User Authentication**: Secure authentication via Supabase
- **Responsive UI**: Mobile-friendly interface built with React and Tailwind CSS

##  Architecture

The project is divided into two main components:

### Backend (`Atlas_Wallet_backend/`)
- **Framework**: Python with FastAPI
- **AI Integration**: LangChain-based agent graph for intelligent shopping assistance
- **Services**: Cart, wallet, purchase, search, and context management
- **Database**: Supabase integration for data persistence
- **APIs**: RESTful endpoints for catalog, wallet, and agent operations

### Frontend (`atlas_wallet_frontend/`)
- **Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS with shadcn/ui components
- **State Management**: React Query for server state
- **Build Tool**: Vite
- **Testing**: Vitest for unit tests
- **Authentication**: Supabase authentication integration

##  Getting Started

### Prerequisites
- Node.js 20+ and npm/bun
- Python 3.9+
- Git

### Backend Setup

1. Navigate to the backend directory:
```bash
cd Atlas_Wallet_backend
```

2. Install dependencies:
```bash
pip install -r pyproject.toml
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your configuration
```

4. Run the backend server:
```bash
python server.py
```

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd atlas_wallet_frontend
```

2. Install dependencies:
```bash
npm install
# or
bun install
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your Supabase configuration
```

4. Start the development server:
```bash
npm run dev
```

5. Build for production:
```bash
npm run build
```

##  Project Structure

```
Atlas_Wallet/
├── Atlas_Wallet_backend/          # Python backend
│   ├── api/                        # API routes
│   ├── app/                        # Core application logic
│   │   ├── agent/                  # AI agent implementation
│   │   └── services/               # Business logic services
│   ├── mocks/                      # Mock data
│   └── server.py                   # Main server entry point
├── atlas_wallet_frontend/          # React frontend
│   ├── src/
│   │   ├── components/             # React components
│   │   ├── pages/                  # Page components
│   │   ├── hooks/                  # Custom React hooks
│   │   ├── lib/                    # Utility functions
│   │   └── integrations/           # Third-party integrations
│   └── supabase/                   # Supabase functions and migrations
├── Dockerfile                      # Container configuration
└── README.md                       # This file
```

##  Technologies Used

### Backend
- Python 3.9+
- FastAPI
- LangChain
- Supabase
- Docker

### Frontend
- React 18
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui
- React Query
- React Router

##  Testing

Run tests for the frontend:
```bash
npm run test              # Run tests once
npm run test:watch       # Run tests in watch mode
```

##  Available Scripts

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run test` - Run tests
- `npm run test:watch` - Run tests in watch mode

##  Deployment

The project includes Railway deployment configuration via `railway.toml` and a `Dockerfile` for containerization.

To deploy on Railway:
1. Push your code to GitHub
2. Connect your repository to Railway
3. Configure environment variables
4. Deploy

See [RAILWAY_DEPLOY.md](RAILWAY_DEPLOY.md) for detailed deployment instructions.

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

##  Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions or support, please open an issue on GitHub.
