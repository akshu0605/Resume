# 3D Personal Portfolio Website

A high-performance, interactive personal portfolio website built with React, Vite, and Tailwind CSS, featuring 3D elements and smooth animations.

## 🚀 Features

- **Interactive UI**: Utilizing `framer-motion` for fluid animations and `lucide-react` for iconography.
- **Responsive Design**: Fully responsive layout optimized for all device sizes using Tailwind CSS.
- **3D Elements**: Interactive 3D components and custom cursors for an immersive experience.
- **Backend Integration**: Supabase integration for visitor tracking and contact form submissions.
- **Optimized Performance**: Vite-powered build for lightning-fast development and production, now configured for Vercel edge capabilities.

## 🛠️ Tech Stack

- **Framework**: React 18
- **Build Tool**: Vite
- **Styling**: Tailwind CSS, `clsx`, `tailwind-merge`
- **Animations**: Motion (Framer Motion)
- **UI Components**: Radix UI primitives, `sonner` for toasts
- **Backend**: Supabase (Edge Functions)
- **Deployment**: Vercel

## 📦 Installation

1.  **Clone the repository**:
    ```bash
    git clone <your-repo-url>
    cd my-website-max
    ```

2.  **Install dependencies**:
    ```bash
    npm install
    ```

3.  **Environment Setup**:
    Create a `.env` file in the root directory (optional, for local development overrides):
    ```env
    VITE_SUPABASE_URL=your_supabase_url
    VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
    ```
    *Note: Current supabase info is hardcoded in `src/utils/supabase/info.js` for simplicity, but using environment variables is recommended for security.*

## 💻 Usage

- **Start Development Server**:
    ```bash
    npm run dev
    ```
    Runs on [http://localhost:3000](http://localhost:3000).

- **Production Build**:
    ```bash
    npm run build
    ```
    Builds the application to the `dist` folder.

- **Preview Production Build**:
    ```bash
    npm run preview
    ```

## ☁️ Deployment on Vercel

The project is fully configured for seamless deployment on Vercel.

1.  **Push to GitHub/GitLab/Bitbucket**.
2.  **Import Project in Vercel**:
    - Select your repository.
    - Framework Preset: **Vite** (should be auto-detected).
    - Build Command: `npm run build`
    - Output Directory: `dist`
3.  **Deploy**: Click "Deploy" and watch your site go live!

### Vercel Configuration
A `vercel.json` file is included to handle Single Page Application (SPA) routing, ensuring that direct links to sub-routes works correctly.

## 📁 Project Structure

```
├── public/              # Static assets
├── src/
│   ├── components/      # React components
│   │   ├── ui/          # Reusable UI components (buttons, inputs, etc.)
│   │   └── ...          # Feature components (Hero, About, etc.)
│   ├── utils/           # Utility functions and helpers
│   ├── App.jsx          # Main application component
│   ├── main.jsx         # Application entry point
│   └── index.css        # Global styles (Tailwind imports)
├── package.json         # Project dependencies and scripts
├── vite.config.js       # Vite configuration (aliases, plugins)
└── vercel.json          # Vercel deployment configuration
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE).