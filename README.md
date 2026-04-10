# JustInTime – FloatFry Manufacturing Resource Planning

> A web-based Manufacturing Resource Planning (MRP) system built for FloatFry, premium non-stick cookware manufacturer. Developed as part of the 5005CMD Software Engineering module at Coventry University.

---

## Project Overview

FloatFry operates on a strict Just-in-Time (JIT) production philosophy. This system digitises and automates their manufacturing lifecycle, covering machine monitoring, operator job scheduling, order management, and production tracking across multiple user roles.

---

## Built With

- React.js 18
- React Router v6
- Plain CSS (no external UI library)
- JavaScript (ES6+)

---

## Features

- Role-based login (Floor Manager, Stamper, Production Manager)
- Real-time machine status dashboard with colour-coded indicators
- Stamper job sheet with materials-ready toggle per job card
- Production schedule and order management table
- Notification panel for critical alerts
- Filter functionality across all dashboards
- Fully responsive layout

---

## Prerequisites

Make sure you have the following installed before running the project:

| Software | Version | Download |
|---|---|---|
| Node.js | v18.x or higher | https://nodejs.org |
| npm | v9.x or higher (comes with Node.js) | Included |
| Git | Latest | https://git-scm.com |

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/opokua7/JustInTime_FloatFry.git
```

### 2. Navigate into the project folder

```bash
cd justintime
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm start
```

### 5. Open in browser

The app will open automatically at:

```
http://localhost:3000
```

If it does not open automatically, open your browser and navigate to the URL above.

---

## Login Credentials

Use the following credentials to access each role-specific dashboard:

| Role | Username | Password |
|---|---|---|
| Floor Manager | `floormanager` | `Floor@1234` |
| Stamper | `stamper01` | `Stamp@1234` |
| Production Manager | `prodmgr` | `ProdMgr@1234` |

---

## Project Structure

```
justintime-mrp/
├── public/
│   └── index.html
├── src/
│   ├── App.js               # Main router and app entry point
│   ├── App.css              # Global styles
│   ├── components/
│   │   └── Navbar.js        # Shared navigation bar
│   └── pages/
│       ├── Login.js         # Login page with role-based routing
│       ├── FloorManager.js  # Machine status dashboard
│       ├── StamperJobSheet.js  # Stamper job sheet and job cards
│       └── ProductionManager.js  # Production schedule and orders
├── package.json
└── README.md
```

---

## Available Scripts

### `npm start`
Runs the app in development mode at `http://localhost:3000`. The page reloads automatically when you make changes.

### `npm test`
Launches the test runner in interactive watch mode.

### `npm run build`
Builds the app for production into the `build/` folder. The build is minified and optimised for best performance.

---

## User Roles and Access

### Floor Manager
- View real-time machine status dashboard
- Monitor cycle progress per machine
- See colour-coded status indicators (Running / Maintenance Due / Fault / Idle)
- View recent notifications

### Stamper
- Clock in and view personalised daily job sheet
- See job cards with machine, location, time, design pattern, materials, certification required
- Toggle materials-ready confirmation per job card
- Filter jobs by status

### Production Manager
- View full order list with status tracking
- Filter orders by status (Pending / In Production / Completed / Issue)
- Monitor delivery timelines and customisation details




