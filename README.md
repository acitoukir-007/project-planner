# Task & Resource Planner (macOS Sonoma Edition)

A high-performance, single-page web application for task management, Gantt scheduling, and resource planning with a sleek macOS Sonoma glassmorphic UI.

---

## 💻 Local Usage

You can continue opening the app locally anytime via your browser:

```text
file:///D:/Project%20planner/index.html
```

Your local file path, offline capabilities, and saved data remain completely unchanged.

---

## 🚀 How to Host on GitHub & Vercel

Follow either **Method 1** (Browser UI - No installation needed) or **Method 2** (Git CLI).

### Method 1: Web Interface (Simplest & Fastest)

#### Step 1: Create a GitHub Repository
1. Log in to [GitHub](https://github.com).
2. Click the **`+`** icon in the top right corner and select **New repository**.
3. Name it (e.g. `project-planner`).
4. Set the visibility to **Public** or **Private**.
5. Leave "Add a README file" unchecked (we already have one).
6. Click **Create repository**.

#### Step 2: Upload Files to GitHub
1. On the new repository page, click **uploading an existing file**.
2. Drag and drop these files from `D:\Project planner`:
   - `index.html`
   - `vercel.json`
   - `package.json`
   - `.gitignore`
   - `README.md`
   *(Do **not** upload the `.bak` backup files)*
3. Click **Commit changes**.

#### Step 3: Deploy to Vercel
1. Log in to [Vercel](https://vercel.com) (you can log in using your GitHub account).
2. Click **Add New...** → **Project**.
3. Find your `project-planner` repository under "Import Git Repository" and click **Import**.
4. In the Project Configuration:
   - **Framework Preset**: Select `Other` (Static HTML).
   - **Root Directory**: `./` (Default).
5. Click **Deploy**.
6. Within 15-30 seconds, Vercel will give you a live production URL (e.g., `https://project-planner-xyz.vercel.app`).

---

### Method 2: Using Git CLI (Optional)

If you prefer using the command line:

1. **Install Git** (if not already installed):
   ```powershell
   winget install --id Git.Git -e --source winget
   ```
2. **Initialize and push**:
   ```powershell
   cd "D:\Project planner"
   git init
   git add index.html vercel.json package.json .gitignore README.md
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. Connect the repository to [Vercel](https://vercel.com) as described in Method 1.

---

## 🔒 Notes on Data Storage
- All tasks, Gantt data, and notes are saved locally in the browser's `localStorage` (`TRP_APP_DATA`).
- When accessing the app via Vercel online, data is securely stored in your browser session for that domain.
- You can export your data anytime from the interface.
