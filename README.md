# WIUT Student Research Paper Portal

A responsive web portal for Westminster International University in Tashkent (WIUT) students to submit research papers and for faculty/administrators to manage submissions with Excel export capabilities.

## 🚀 Features

- **Student Submission Form**:
  - Student details validation (ID format validation `000xxxxx`, `@wiut.uz` email verification).
  - Academic field categorization.
  - Abstract & research paper file upload (PDF, DOC, DOCX).
  - Instant submission receipt modal.
- **Admin Management Panel**:
  - Secure passcode-protected admin access (`Muno123`).
  - Search and filter student submissions in real-time.
  - Export submission records to formatted Excel spreadsheets (`.xlsx`) using SheetJS.
- **Production-Ready Styling**:
  - Built with [Tailwind CSS](https://tailwindcss.com/) (minified, standalone CSS).
  - Responsive design with smooth animations.
  - Icons powered by [Lucide Icons](https://lucide.dev/).

---

## 🛠️ Local Development

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Start Tailwind CSS in watch mode**:
   ```bash
   npm run dev
   ```

3. **Build minified CSS for production**:
   ```bash
   npm run build
   ```

4. Open `index.html` in your web browser (or serve with any local HTTP server like `npx serve .` or VS Code Live Server).

---

## 🌐 GitHub Pages Deployment

### Option 1: Automated Deployment via GitHub Actions (Recommended)
This repository includes a GitHub Actions workflow (`.github/workflows/deploy.yml`) that automatically builds Tailwind CSS and deploys to GitHub Pages on push to `main`.

1. Go to repository **Settings** -> **Pages**.
2. Under **Build and deployment** > **Source**, select **GitHub Actions**.
3. Pushes to `main` will trigger the deployment automatically.

### Option 2: Deploy from Branch
Since the compiled production CSS is saved in `css/style.css`, you can also deploy directly:
1. Go to repository **Settings** -> **Pages**.
2. Under **Build and deployment** > **Source**, select **Deploy from a branch**.
3. Choose branch `main` and folder `/ (root)`.
