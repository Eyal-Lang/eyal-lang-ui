# EyalLang UI

A static website for the EyalLang project - a rule-based Python DSL.

## 🚀 GitHub Pages Setup

This repository is configured to automatically deploy to GitHub Pages using GitHub Actions. Here's how to set it up:

### 1. Enable GitHub Pages

1. Go to your repository on GitHub
2. Navigate to **Settings** > **Pages**
3. Under "Source", select **GitHub Actions**
4. The workflow will automatically deploy your site when you push to the `main` branch

### 2. Repository Settings

Make sure your repository has the following settings:
- **Public repository** (required for GitHub Pages on free accounts)
- **Actions enabled** (should be enabled by default)

### 3. Deploy

1. Commit and push your changes to the `main` branch:
   ```bash
   git add .
   git commit -m "Initial commit with GitHub Pages workflow"
   git push origin main
   ```

2. The GitHub Actions workflow will automatically:
   - Build the site from the `src/` directory
   - Deploy it to GitHub Pages
   - Your site will be available at `https://<username>.github.io/<repository-name>`

## 📁 Project Structure

```
eyal-lang-ui/
├── .github/workflows/
│   └── deploy.yml          # GitHub Actions workflow
├── src/
│   └── index.html          # Main website file
└── README.md               # This file
```

## 🔄 Workflow Details

The GitHub Actions workflow (`deploy.yml`) will:
- Trigger on pushes to the `main` branch
- Deploy the contents of the `src/` directory to GitHub Pages
- Use the latest GitHub Pages actions for optimal performance

## 🛠 Local Development

To work on the site locally:
1. Open `src/index.html` in your browser
2. Make changes to the HTML file
3. Commit and push to deploy automatically

## 📝 Notes

- The workflow deploys the entire `src/` directory
- Changes to the `main` branch automatically trigger a new deployment
- GitHub Pages may take a few minutes to reflect changes 