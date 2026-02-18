# React Runner Circle

A React application for tracking running workouts and sharing them with a community feed. Built with Vite, Apollo GraphQL Client, and Tailwind CSS.

## Prerequisites

- Node.js (v16 or higher)
- npm

## Quick Start

Follow these steps to get the application up and running:

### 1. Install Dependencies

```bash
npm install
```

### 2. Start the GraphQL Server

Open a terminal and run the local GraphQL server:

```bash
npm run server:json-graphql
```

The server will be running on `http://localhost:3001`

### 3. Run the Development Server

Open another terminal and start the development server:

```bash
npm run dev
```

The application will be available at `http://localhost:5173` (or the port shown in your terminal)

## Available Scripts

- `npm run dev` - Start the Vite development server with hot module replacement
- `npm run build` - Build the application for production
- `npm run preview` - Preview the production build locally
- `npm run lint` - Run ESLint to check code quality
- `npm run server:json-server` - Run a JSON server (alternative to GraphQL server)
- `npm run server:json-graphql` - Run the JSON GraphQL server

## Project Structure

```
src/
├── pages/           # Page components (Feed, NewPost, Login, etc.)
├── components/
│   ├── layout/      # Layout components (Header, Sidebar, etc.)
│   ├── forms/       # Form components (LoginForm, NewPostForm, etc.)
│   └── ui/          # Reusable UI components (Button, Card, Input, etc.)
├── assets/          # Static assets
├── App.jsx          # Main App component
├── main.jsx         # Entry point
└── index.css        # Global styles

database/
├── json-graphql-server.js  # GraphQL server configuration
├── json-server.json        # JSON server data
└── graphql/
    ├── query/       # GraphQL query definitions
    └── mutation/    # GraphQL mutation definitions
```

## Technology Stack

- **React** - UI library
- **Vite** - Build tool and dev server
- **Apollo Client** - GraphQL client
- **Tailwind CSS** - Utility-first CSS framework
- **Material-UI (MUI)** - Component library
- **json-graphql-server** - Local GraphQL backend

## Development

The application uses Apollo Client to manage state and communicate with the GraphQL server. The cache is automatically updated when mutations are performed.

### Making Changes

1. Edit files in `src/`
2. Changes will automatically hot-reload in your browser
3. Check the browser console for any errors

## Building for Production

```bash
npm run build
npm run preview
```

The optimized build will be created in the `dist/` folder.

## License

MIT
