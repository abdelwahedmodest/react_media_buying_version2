# Media Buying Frontend

This is the React frontend for the Media Buying project. It's built with React, Vite, and Tailwind CSS.

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development server:
   ```bash
   npm run dev
   ```

The development server will run at `http://localhost:5173/`.

## Build for Production

To build the frontend for production:

```bash
npm run build
```

The build output will be in the `dist` directory.

## API Configuration

The frontend is configured to communicate with the Django backend API at `http://127.0.0.1:8000/api`. If you need to change this configuration, update the `baseURL` in `src/services/api.js`.

## Project Structure

```
frontend/
├── src/
│   ├── components/     # Reusable UI components
│   ├── contexts/       # React context providers
│   ├── i18n/           # Internationalization files
│   ├── pages/          # Page components
│   ├── services/       # API services
│   ├── App.jsx         # Main application component
│   ├── main.jsx        # Entry point
│   └── index.css       # Global styles
├── public/             # Static assets
└── index.html          # HTML template
```

## Features

- React Router for navigation
- Axios for API requests
- Tailwind CSS for styling
- Internationalization support