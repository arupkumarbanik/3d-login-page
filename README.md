<div align="center">

# 🪐 NEURA — 3D Animated Authentication Experience

**A cutting-edge, responsive 3D animated SaaS authentication portal built with pure HTML5, CSS3, and Vanilla JavaScript. Zero external frameworks. Zero 3D canvas libraries. Pure web craftsmanship.**

[![GitHub Repo](https://img.shields.io/badge/GitHub-love--login--page-blue?logo=github)](https://github.com/arupkumarbanik/love-login-page)
[![Live Demo](https://img.shields.io/badge/Live-GitHub%20Pages-success?logo=githubpages&logoColor=white)](https://arupkumarbanik.github.io/love-login-page/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Author](https://img.shields.io/badge/Author-Arup%20Kumar%20Banik-purple?logo=github)](https://github.com/arupkumarbanik)

[🌐 Live Demo](https://arupkumarbanik.github.io/love-login-page/) • [✨ Features](#-key-features) • [🚀 Quick Start](#-quick-start-run-locally) • [🌍 Deployment Guide](#-deployment-guide) • [🎨 Customization](#-customization-guide) • [👨‍💻 Author](#-author)

</div>

---

## 📖 Project Overview

**NEURA** is a production-grade, cyberpunk-inspired authentication experience designed for modern SaaS applications, developer platforms, and AI intelligence dashboards. 

Unlike conventional login pages that rely on heavy 3D rendering engines (such as Three.js, WebGL, or Canvas bundles weighing multiple megabytes), **NEURA** achieves hyper-smooth, cinematic 3D visual depth purely through **CSS 3D transforms (`transform-style: preserve-3d`), hardware acceleration, and a sub-millisecond linear interpolation (LERP) mouse parallax engine written in Vanilla JavaScript**.

Whether you are integrating it into an existing full-stack web application, embedding it as a landing page gate, or showcasing it in your developer portfolio, NEURA runs seamlessly in every modern browser with instant zero-second load times.

---

## ✨ Key Features

### 🌌 1. Pure CSS3 3D Holographic Stage
- **Multi-Layered Glass Orb Core**: Features radial specular highlights, an animated swirling plasma core (`plasmaSwirl`), inner glow reflections, and pulsating ambient bloom.
- **Concentric Orbiting Neon Rings**: Three independent multi-axial gyroscope rings with glowing orbital satellites rotating in 3D perspective (`rotateX`, `rotateY`, `rotateZ`).
- **Floating 3D Polyhedra**: Fully synthesized 3D objects including a 6-faced wireframe cube, an octahedron gem, a glowing energy tetrahedron, and a spinning torus ring.
- **Ambient Space Canvas**: Atmospheric aurora mesh gradients, cybernetic grid floor with radial masking, and twinkling ambient micro-stars.

### 🕹️ 2. Hardware-Accelerated 60 FPS Parallax Engine
- **Linear Interpolation (LERP)**: Mouse movement coordinates are normalized `[-1, 1]` and smoothly smoothed at 60 FPS via `requestAnimationFrame` for buttery-soft depth sensation without pointer lag.
- **Multi-Depth Visual Layering**: The orb, ambient backplate, floating geometries, and background auroras move at varying parallax speeds (`translate3d`).
- **3D Card Tilt & Specular Spotlight**: The authentication card dynamically tilts in response to cursor position while updating CSS custom variables (`--mouse-x`, `--mouse-y`) to sweep a realistic glass glare highlight across the card surface.

### 🔄 3. Seamless 3D Form Transitions
- **Card Flip & Depth Cascade**: Effortlessly toggles between **Sign In** and **Create Account** forms with a 3D depth flip effect.
- **Staggered Entrance Delays**: Form inputs and CTA components cascade into view using micro-timed entrance keyframes (`fadeInUp`).
- **Auto Focus Management**: Automatically transfers focus to the primary input field of the active form for optimal UX.

### 🔒 4. Real-Time Client Validation & Feedback
- **Dynamic Password Strength Meter**: Live 4-tier security evaluation (**Weak** $\rightarrow$ **Fair** $\rightarrow$ **Good** $\rightarrow$ **Strong**) with real-time criteria checks (8+ characters, uppercase, number, symbol).
- **Comprehensive Validation Rules**: Email pattern syntax check, password confirmation matching, mandatory terms check, and inline animated warning text.
- **Password Visibility Toggles**: Custom SVG eye open/closed icons with accessible state toggling.
- **Interactive Button States**: Primary CTA buttons feature a glowing hover layer, diagonal light sweep effect, and animated circular spinner loader during simulated asynchronous submission.

### 🪟 5. Modal & Notification Engines
- **Forgot Password Recovery Modal**: Accessible glassmorphic dialog with backdrop blur, keyboard dismissal (`Esc`), focus trapping, and recovery token transmission simulation.
- **Toast Notification Engine**: Animated floating toast notifications with success and error styling, auto-dismiss timers, and `aria-live="assertive"` screen-reader announcements.

### 📱 6. Responsive & Accessible
- **Mobile & Tablet Optimized**: Collapses into a single-column layout on smaller screens, scaling down the 3D scene into an ambient decorative banner while keeping 44px+ touch-friendly inputs and buttons.
- **Reduced Motion Support**: Fully respects `@media (prefers-reduced-motion: reduce)` by disabling infinite rotations and intensive parallax calculations.

---

## 🗂️ File Structure

```text
neura-auth/
├── index.html           # Main semantic HTML5 markup & accessible form structures
├── style.css            # Complete design system: 3D transforms, animations & glassmorphism
├── script.js            # Pure Vanilla JS: LERP parallax, form validation, modal & toast
├── package.json         # Optional Vite/Node tooling for modern development pipelines
├── vite.config.ts       # Optional Vite configuration
├── metadata.json        # Project metadata
├── .env.example         # Environment template
├── .gitignore           # Git ignore rules
└── README.md            # Project documentation & deployment guide
```

> **Note**: Because this project uses standard web technologies, **`index.html`**, **`style.css`**, and **`script.js`** can be opened directly or served statically without any build process!

---

## 🚀 Quick Start (Run Locally)

You can run this project locally using whichever method fits your workflow best:

### Method 1: Instant Static Launch (No Node.js Required)
Simply double-click `index.html` in your file manager to open it in any web browser, or use one of these lightweight local servers:

* **Using Python 3:**
  ```bash
  python3 -m http.server 3000
  ```
  Open `http://localhost:3000` in your browser.

* **Using VS Code Live Server Extension:**
  Right-click `index.html` inside VS Code and select **"Open with Live Server"**.

* **Using `npx serve`:**
  ```bash
  npx serve .
  ```

---

### Method 2: Using Node.js & Vite (Included Tooling)
If you prefer a modern developer workflow with hot-reloading:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/arupkumarbanik/love-login-page.git
   cd love-login-page
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```
   Open `http://localhost:3000` in your browser.

4. **Generate a production build:**
   ```bash
   npm run build
   ```
   The compiled assets will be placed in the `dist/` directory.

---

## 🌐 Deployment Guide

Deploying NEURA takes less than 2 minutes. Choose your preferred hosting provider below:

### 1. Deploying to GitHub Pages (Recommended - 100% Free)

#### Method A: Direct Deployment from Branch
1. Push your code to your GitHub repository:
   ```bash
   git add .
   git commit -m "feat: initial commit with NEURA 3D auth"
   git push origin main
   ```
2. Navigate to your repository on GitHub.
3. Click on **Settings** $\rightarrow$ **Pages** (in the left sidebar).
4. Under **Build and deployment** $\rightarrow$ **Source**, choose **Deploy from a branch**.
5. Select branch: `main` and folder: `/ (root)`.
6. Click **Save**. Within 1–2 minutes, your live URL will be active at:
   👉 **`https://arupkumarbanik.github.io/love-login-page/`**

#### Method B: GitHub Actions (Automated Vite Build)
If you build the project via `npm run build`:
1. Create a file `.github/workflows/deploy.yml`:
   ```yaml
   name: Deploy to GitHub Pages

   on:
     push:
       branches: [main]

   permissions:
     contents: read
     pages: write
     id-token: write

   concurrency:
     group: 'pages'
     cancel-in-progress: true

   jobs:
     deploy:
       environment:
         name: github-pages
         url: ${{ steps.deployment.outputs.page_url }}
       runs-on: ubuntu-latest
       steps:
         - name: Checkout
           uses: actions/checkout@v4
         - name: Setup Node
           uses: actions/setup-node@v4
           with:
             node-version: 20
         - name: Install dependencies
           run: npm ci
         - name: Build static site
           run: npm run build
         - name: Setup Pages
           uses: actions/configure-pages@v4
         - name: Upload artifact
           uses: actions/upload-pages-artifact@v3
           with:
             path: './dist'
         - name: Deploy to GitHub Pages
           id: deployment
           uses: actions/deploy-pages@v4
   ```

---

### 2. Deploying to Vercel

#### Method A: Via Vercel Dashboard (Zero Config)
1. Go to [Vercel](https://vercel.com) and log in.
2. Click **"Add New..."** $\rightarrow$ **"Project"**.
3. Import your GitHub repository.
4. If deploying static root files:
   - **Framework Preset**: `Other`
   - **Root Directory**: `./`
   - Click **Deploy**.
5. If deploying via Vite:
   - **Framework Preset**: `Vite`
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
   - Click **Deploy**.

#### Method B: Via Vercel CLI
```bash
npm i -g vercel
vercel
```

---

### 3. Deploying to Netlify

#### Method A: Git Integration
1. Visit [Netlify](https://www.netlify.com) and log in.
2. Click **"Add new site"** $\rightarrow$ **"Import an existing project"**.
3. Select GitHub and authorize your repository.
4. Configure build settings:
   - **Publish directory**: `.` (or `dist` if using Vite build)
   - **Build command**: Leave blank for static, or `npm run build`
5. Click **"Deploy site"**.

#### Method B: Drag and Drop
1. Open the Netlify **Sites** page.
2. Drag and drop the project folder directly into the Netlify web UI for instantaneous hosting.

---

### 4. Deploying with Docker & Nginx

For self-hosted servers, Kubernetes, or containerized clouds (AWS ECS, Google Cloud Run, Azure Container Apps):

1. **Create a `Dockerfile`:**
   ```dockerfile
   FROM nginx:alpine
   COPY index.html /usr/share/nginx/html/
   COPY style.css /usr/share/nginx/html/
   COPY script.js /usr/share/nginx/html/
   EXPOSE 80
   CMD ["nginx", "-g", "daemon off;"]
   ```

2. **Build and run the container:**
   ```bash
   docker build -t neura-auth .
   docker run -d -p 8080:80 neura-auth
   ```
   Access the app at `http://localhost:8080`.

---

## 🎨 Customization Guide

### Changing the Color Scheme
All colors, glow radiuses, and glass gradients are defined as standard CSS Custom Properties inside the `:root` pseudo-class in `style.css`:

```css
:root {
  /* Brand Primary & Glows */
  --primary-purple: #8b5cf6;
  --primary-purple-glow: rgba(139, 92, 246, 0.45);
  --primary-purple-deep: #6d28d9;

  /* Secondary Accent */
  --secondary-cyan: #06b6d4;
  --secondary-cyan-glow: rgba(6, 182, 212, 0.45);
  --secondary-cyan-bright: #38bdf8;

  /* Status Colors */
  --accent-emerald: #10b981;  /* Success & Strong passwords */
  --accent-rose: #f43f5e;     /* Errors & Weak passwords */
  --accent-amber: #f59e0b;    /* Warning & Fair passwords */
}
```

* To create an **Emerald / Cyberpunk Green** theme: replace `--primary-purple` with `#10b981` and `--secondary-cyan` with `#06b6d4`.
* To create an **Amber / Solar Gold** theme: replace `--primary-purple` with `#f59e0b` and `--secondary-cyan` with `#f97316`.

### Connecting Your Real Authentication Backend
The forms in `script.js` include clean asynchronous submission hooks ready to replace the simulated timer with your production REST/GraphQL API:

```javascript
// Inside handleLoginSubmit in script.js:
try {
  const response = await fetch('/api/v1/auth/login', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email, password, remember })
  });

  const data = await response.json();

  if (!response.ok) {
    throw new Error(data.message || 'Authentication failed');
  }

  showToast('Authentication verified. Redirecting...', 'success');
  window.location.href = '/dashboard';
} catch (error) {
  showFormAlert(loginAlert, error.message, 'error');
}
```

---

## 🖥️ Browser Compatibility

| Browser | Supported Version | 3D Engine |
| :--- | :--- | :--- |
| **Google Chrome** | 88+ | Hardware Accelerated (Full 60 FPS) |
| **Mozilla Firefox** | 85+ | Hardware Accelerated (Full 60 FPS) |
| **Apple Safari** | 14+ | WebKit CSS3 3D (Full 60 FPS) |
| **Microsoft Edge** | 88+ | Chromium Engine (Full 60 FPS) |
| **iOS Safari** | 14+ | Touch Parallax & Responsive Layout |
| **Android Chrome** | 88+ | Touch Parallax & Responsive Layout |

---

## 🤝 Contributing

Contributions, feedback, and pull requests are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/FuturisticTheme`)
3. Commit your changes (`git commit -m 'Add futuristic neon gold theme'`)
4. Push to the branch (`git push origin feature/FuturisticTheme`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Arup Kumar Banik**
- GitHub: [@arupkumarbanik](https://github.com/arupkumarbanik)
- Repository: [love-login-page](https://github.com/arupkumarbanik/love-login-page)
- Live Deployment: [https://arupkumarbanik.github.io/love-login-page/](https://arupkumarbanik.github.io/love-login-page/)

---

## 📄 License

This project is open-source and released under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute this template in personal or commercial projects.

---

<div align="center">
  <sub>Engineered with precision for modern web artisans. Maintained by <a href="https://github.com/arupkumarbanik">Arup Kumar Banik</a>. If this project inspires you, consider starring ⭐ the repository!</sub>
</div>
