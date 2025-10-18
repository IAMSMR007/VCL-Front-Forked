# VirtualChemLab Frontend

## Overview
A React-based virtual chemistry lab interface application built with Vite. This project provides a web-based platform for simulating chemistry lab experiences with user authentication and interactive lab features.

**Current State:** Fully functional and ready to use in Replit environment.

**Last Updated:** October 18, 2025

## Project Architecture

### Technology Stack
- **Frontend Framework:** React 18
- **Build Tool:** Vite 5
- **Routing:** React Router DOM v7
- **Development Server:** Vite dev server on port 5000

### Project Structure
```
├── src/
│   ├── Features/
│   │   ├── Auth/           # Authentication pages
│   │   ├── Hero/           # Landing/hero page
│   │   └── LabInterface/   # Main lab interface
│   ├── App.jsx             # Main app with routing
│   └── main.jsx            # React app entry point
├── index.html              # HTML template
├── vite.config.js          # Vite configuration
└── package.json            # Dependencies
```

### Routes
- `/` - Hero/landing page
- `/auth` - Authentication page
- `/lab` - Interactive lab interface with full chemistry simulation features

## Replit Configuration

### Vite Configuration
The project is configured for Replit's environment with:
- Host binding to `0.0.0.0:5000`
- HMR over WSS on port 443
- Proxy configuration for API calls to `/api` endpoints (backend at localhost:5000 if present)

### Workflow
- **Server:** Runs `npm run dev` to start the Vite development server on port 5000

## Development

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

### Dependencies
Production:
- react ^18.0.0
- react-dom ^18.0.0
- react-router-dom ^7.9.4

Development:
- @vitejs/plugin-react ^4.0.0
- vite ^5.0.0

## Features

### Lab Interface (`/lab`)
The main lab interface provides a complete virtual chemistry lab experience:

**Workbench Panel:**
- Interactive test tube visualization with animations
- Experiment/Prediction mode tabs
- Unknown Salt A sample analysis
- Action buttons: Heat, Filter, Dilute, Wait

**Reagent Shelf:**
- 6 interactive reagent cards with selectable chemistry compounds
- Silver Nitrate (AgNO₃), Hydrochloric Acid (HCl), Sodium Hydroxide (NaOH)
- Sulfuric Acid (H₂SO₄), Sodium Carbonate (Na₂CO₃), Ammonia Solution (NH₃)
- All reagents at 0.1M concentration

**Recent Steps Tracking:**
- Timestamped log of all actions
- Undo functionality to reverse steps
- Real-time updates as actions are performed

**Log System:**
- Three-tab interface: Log, Notes, Results
- Detailed experiment log with timestamps
- Tracks reagent additions and observations

**Keyboard Shortcuts:**
- Quick access to common lab actions
- Visual reference bar at bottom of interface

## Recent Changes
- **2025-10-18:** Created complete lab interface with interactive workbench, reagent shelf, and logging system
- **2025-10-18:** Added real-time step tracking and undo functionality
- **2025-10-18:** Implemented responsive three-panel layout with dark theme
- **2025-10-18:** Configured Vite for Replit environment (host binding, HMR settings)
- **2025-10-18:** Set up workflow for development server
- **2025-10-18:** Installed dependencies and verified application functionality
