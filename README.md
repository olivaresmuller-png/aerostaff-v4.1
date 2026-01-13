# Asset Analyzer

A comprehensive asset analysis and management tool built with React, Vite, Express, and PostgreSQL.

## Features

- **Dashboard**: Overview of total value, asset categories, and active alerts.
- **Asset Management**: Add, edit, and track assets with details like cost, scrap value, and useful life.
- **Depreciation Calculation**: Real-time calculation of asset depreciation (Straight Line & Double Declining methods).
- **Reports**: Generate reports including Asset List, Depreciation Schedule, and Net Value/ROI Analysis.
- **Data Import/Export**: Import assets from CSV/Excel and export reports.
- **Settings**: Configure default methods, alerts, and user preferences.
- **Admin**: User management and system audit logs.

## Tech Stack

- **Frontend**: React 19, Vite, TailwindCSS (v4), Radix UI, Framer Motion, Recharts.
- **Backend**: Node.js, Express.
- **Database**: PostgreSQL with Drizzle ORM.
- **Language**: TypeScript throughout the stack.

## Prerequisites

- Node.js (v20 or later recommended)
- PostgreSQL Database

## Setup

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd Asset-Analyzer
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Variables:**
    Copy `.env.example` to `.env` and fill in your database credentials.
    ```bash
    cp .env.example .env
    ```
    Update `DATABASE_URL` in `.env`.

4.  **Database Migration:**
    Push the schema to your database.
    ```bash
    npm run db:push
    ```

5.  **Run Development Server:**
    ```bash
    npm run dev
    ```
    This starts the backend server, which also serves the frontend in development mode.

## Scripts

- `npm run dev`: Start the development server.
- `npm run build`: Build the frontend and backend for production.
- `npm run start`: Start the production server.
- `npm run check`: Run TypeScript type checking.
- `npm run db:push`: Push Drizzle schema changes to the database.
