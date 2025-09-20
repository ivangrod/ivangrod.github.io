# Needlehack

Needlehack is a blog deployed on **GitHub Pages** using **Jekyll** and **Tailwind CSS**.  
It focuses on sharing product development journeys.

---

## 🚀 Features
- Static blog powered by **Jekyll**
- Styled with **Tailwind CSS**
- Automatic deployment with **GitHub Actions**
- Interactive graphs with **vis-network**
- Pages:
  - **Landing page** (short introduction)
  - **Journeys → Philiapp → Creating our first iteration**
  - **Interactive graph** with nodes linking to:
    - *The first MVP*
    - *Our architecture*
  - **About Us** (placeholder for now)

---

## 📦 Local Development

### 1. Install dependencies
You need **Ruby**, **Bundler**, **Node.js**, and **npm** installed.

```bash
bundle install
npm install
```

### 2. Build CSS (Tailwind)
To build the Tailwind CSS:

```bash
npm run build:css
```

To watch for changes while developing:

```bash
npm run watch:css
```

### 3. Run Jekyll locally
Serve the site with hot reload:

```bash
npm run serve
```

Then open [http://localhost:4000](http://localhost:4000).

---

## 🌐 Deployment
Deployment is automated via **GitHub Actions**.  
On every push to the `main` branch, GitHub will:
1. Install Ruby and Node.js dependencies
2. Build Tailwind CSS
3. Build the Jekyll site
4. Deploy to **GitHub Pages**

You can check deployment logs under **Actions** in your repository.

---

## 📂 Project structure
```
needlehack/
├── _config.yml
├── Gemfile
├── package.json
├── tailwind.config.js
├── _layouts/default.html
├── index.html
├── about.html
├── journeys/philiapp.html
├── iterations/creating-first-iteration.html
├── posts/
│   ├── mvp.html
│   └── architecture.html
├── assets/css/tailwind.css
├── assets/images/
└── .github/workflows/deploy.yml
```

---

## 📜 License
MIT License
