# ⚡ Vega Server Panel

Real-time server management and monitoring dashboard

A modern, animated server panel built with React, Tailwind CSS, and Lucide React. Features a beautiful hexagonal logo, smooth animations, and a clean black & white design.

## 🌟 Features

🎨 **Animated Logo**: Hexagonal design with clean aesthetics
📱 **Responsive Design**: Mobile-first with collapsible sidebar
✨ **Interactive Elements**: Button scaling effects and hover animations
📊 **Server Management**: Real-time monitoring, controls, and statistics
🎯 **Modern UI**: Minimalist black & white theme with smooth transitions
⚡ **Performance**: Optimized for fast loading and smooth interactions
🔥 **Interactive Controls**: Start/stop servers, view metrics, and manage settings

## 🚀 Quick Start

### Prerequisites

- Bun installed on your system ([Install Bun](https://bun.sh/))
- Node.js 16+ (if using npm/yarn instead of Bun)

### One-Line Setup
```bash
mkdir vega-server-panel && cd vega-server-panel && bun init -y && bun add react react-dom lucide-react && bun add -d vite @vitejs/plugin-react tailwindcss postcss autoprefixer && bunx tailwindcss init -p
```

### Step-by-Step Installation

1. **Create Project Directory**
```bash
mkdir vega-server-panel
cd vega-server-panel
```

2. **Initialize Project**
```bash
bun init -y
```

3. **Install Dependencies**
```bash
# Core dependencies
bun add react react-dom lucide-react

# Development dependencies
bun add -d vite @vitejs/plugin-react tailwindcss postcss autoprefixer
```

4. **Initialize Tailwind CSS**
```bash
bunx tailwindcss init -p
```

## 📁 Project Structure
```
vega-server-panel/
├── public/
├── src/
│   ├── components/
│   │   └── Vega.jsx
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── tailwind.config.js
├── postcss.config.js
├── vite.config.js
└── README.md
```

## ⚙️ Configuration Files

### tailwind.config.js
```javascript
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {
      animation: {
        'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
      },
    },
  },
  plugins: [],
}
```

### vite.config.js
```javascript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'

export default defineConfig({
  plugins: [react()],
  server: {
    port: 3000,
    open: true
  }
})
```

### package.json (scripts section)
```json
{
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview":
