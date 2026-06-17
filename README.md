<div align="center">

<img src="public/logo.png" alt="App Store Logo" width="80" />

# Hero App Store — Single App Detail Page

**A modern, fully responsive app showcase built with React, mimicking the look and feel of a real App Store / Google Play listing.**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-hero--apps--store--ah.netlify.app-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://hero-apps-store-ah.netlify.app/)

![React](https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS_4-06B6D4?style=flat-square&logo=tailwind-css&logoColor=white)
![DaisyUI](https://img.shields.io/badge/DaisyUI-FF69B4?style=flat-square&logo=daisyui&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-FF8042?style=flat-square&logo=chartdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat-square&logo=netlify&logoColor=white)

</div>

---

## Overview

App Store is a React single-page application that replicates the experience of browsing an app marketplace. Users can browse a catalog of apps, view detailed stats for each app (downloads, ratings, reviews), and install apps with a single click — all with a clean, App Store-inspired UI.

---

## Screenshots

| Home                     | App Detail                          | Installed                             |
| ------------------------ | ----------------------------------- | ------------------------------------- |
| ![Hero](public/hero.png) | ![App Detail](public/App-Error.png) | ![Install](public/icon-downloads.png) |

---

## Features

- **App Catalog** — Browse a grid of app cards with icons, titles, categories, and ratings
- **Dynamic App Detail Page** — Each app has its own route (`/apps/:id`) with full details
- **Live Stats** — Total downloads, average rating, and total review count per app
- **Interactive Rating Chart** — Horizontal bar chart (5★ → 1★ breakdown) powered by Recharts
- **Install Button** — Displays app size, saves to `localStorage`, and disables after install
- **Toast Notifications** — Success and error feedback via React Toastify
- **Error Handling** — Redirects to a custom `/error` page when an app ID is not found
- **Loading Spinner** — Shown while fetching app data
- **Fully Responsive** — Mobile, tablet, and desktop layouts using Tailwind CSS + DaisyUI

---

## Tech Stack

| Technology                                                  | Version | Purpose                              |
| ----------------------------------------------------------- | ------- | ------------------------------------ |
| [React](https://react.dev/)                                 | 19      | Component-based UI                   |
| [React Router](https://reactrouter.com/)                    | 7       | Client-side routing & dynamic routes |
| [Tailwind CSS](https://tailwindcss.com/)                    | 4       | Utility-first responsive styling     |
| [DaisyUI](https://daisyui.com/)                             | 5       | Tailwind component library           |
| [Recharts](https://recharts.org/)                           | 3       | Interactive rating bar chart         |
| [React Toastify](https://fkhadra.github.io/react-toastify/) | 11      | Toast notifications                  |
| [Axios](https://axios-http.com/)                            | 1       | HTTP requests                        |
| [Lucide React](https://lucide.dev/)                         | latest  | Icon library                         |
| [Vite](https://vitejs.dev/)                                 | 7       | Build tool & dev server              |

---

## Project Structure

```
src/
├── Components/         # Reusable UI components
│   ├── Banner.jsx
│   ├── Cardsection.jsx
│   ├── Footer.jsx
│   ├── Hero.jsx
│   ├── Navbar.jsx
│   ├── Review.jsx
│   ├── SingleCard.jsx
│   └── Spinner.jsx
├── Hook/               # Custom hooks for data & logic
│   ├── useApps.js      # Fetches app data
│   └── useAppLogic.js  # App detail state & install logic
├── Layouts/
│   └── MainLayout.jsx  # Shared layout with Navbar & Footer
├── Pages/
│   ├── Home.jsx        # Landing page
│   ├── Apps.jsx        # App catalog / browse page
│   ├── AppDetail.jsx   # Single app detail page
│   ├── Install.jsx     # Installed apps list
│   └── ErrorPage.jsx   # 404 / not found page
└── Routes/
    └── Routes.jsx      # Application route definitions
```

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18 or higher
- npm v9 or higher

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/assignment-08.git

# 2. Navigate into the project
cd assignment-08

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

The app will be available at `http://localhost:5173`.

### Available Scripts

| Command           | Description                               |
| ----------------- | ----------------------------------------- |
| `npm run dev`     | Start local development server            |
| `npm run build`   | Build for production (outputs to `dist/`) |
| `npm run preview` | Preview the production build locally      |
| `npm run lint`    | Run ESLint across the project             |

---

## Deployment

This project is deployed on **Netlify** with a `public/_redirects` file to handle client-side routing:

```
/*    /index.html   200
```

To deploy your own instance, push the repository to GitHub and connect it to Netlify. Set the build command to `npm run build` and the publish directory to `dist`.

---

## 📄 License

This project is for portfolio and demonstration purposes.

---

<div align="center">
  Built with ❤️ by <a href="https://github.com/habib-web-dev1">habib-web-dev1</a>
</div>
