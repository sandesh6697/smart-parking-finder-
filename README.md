# Smart Parking Finder

A modern web application for finding and booking parking spots in real-time. Built with React, TypeScript, Vite, and Express.

## Features

- 🗺️ Interactive isometric map with parking spots
- 🔍 Real-time search and filtering
- 📱 Responsive design with mobile support
- 🎤 Voice search functionality
- 📍 GPS location detection
- 💳 Payment processing simulation
- 📊 Admin dashboard for monitoring
- 🌡️ Environment monitoring panel
- ⏱️ Booking timer with notifications

## Tech Stack

- **Frontend:** React 18, TypeScript, Tailwind CSS, Vite
- **Backend:** Express.js, Node.js
- **UI Components:** Radix UI, Lucide Icons
- **State Management:** React Query
- **Testing:** Vitest
- **Deployment:** Netlify (with serverless functions)

## Prerequisites

- Node.js 18+ and npm (or pnpm)
- Git

## Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd smart-parking-finder
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   pnpm install
   ```

## Development

### Start Development Server

```bash
npm run dev
# or
pnpm dev
```

The application will be available at `http://localhost:8080`

### Build for Production

```bash
npm run build
# or
pnpm build
```

This will build both the client and server bundles.

### Start Production Server

```bash
npm start
# or
pnpm start
```

The production server will run on port 3000 by default.

## Testing

Run the test suite:

```bash
npm run test
# or
pnpm test
```

## Code Quality

### Type Checking

```bash
npm run typecheck
# or
pnpm typecheck
```

### Code Formatting

```bash
npm run format.fix
# or
pnpm format.fix
```

## Project Structure

```
├── client/                 # Frontend React application
│   ├── components/         # Reusable UI components
│   ├── pages/             # Page components
│   ├── hooks/             # Custom React hooks
│   ├── lib/               # Utility functions
│   └── types/             # TypeScript type definitions
├── server/                 # Backend Express server
│   ├── routes/            # API route handlers
│   └── index.ts           # Server entry point
├── shared/                 # Shared code between client and server
├── netlify/                # Netlify deployment configuration
│   └── functions/         # Serverless functions
├── public/                 # Static assets
└── dist/                   # Build output (generated)
```

## API Endpoints

- `GET /api/ping` - Health check endpoint
- `GET /api/demo` - Demo endpoint

## Environment Variables

Create a `.env` file in the root directory:

```env
PING_MESSAGE=Hello from Smart Parking Finder
PORT=3000
```

## Deployment

### Netlify

The project is configured for Netlify deployment:

1. Connect your repository to Netlify
2. Set build command: `npm run build:client`
3. Set publish directory: `dist/spa`
4. Configure functions directory: `netlify/functions`

### Docker

Build and run with Docker:

```bash
docker build -t smart-parking-finder .
docker run -p 3000:3000 smart-parking-finder
```

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Make your changes and run tests
4. Commit your changes: `git commit -am 'Add some feature'`
5. Push to the branch: `git push origin feature/your-feature`
6. Submit a pull request

## License

This project is licensed under the MIT License.
