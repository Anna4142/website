# Deploy Your Website to GitHub Pages

## Step 1: Create a New GitHub Repository

1. Go to https://github.com/new
2. Create a repository named `yourusername.github.io` (replace `yourusername` with your GitHub username)
   - For example: `anushkadeshpande.github.io` or `Anna4142.github.io`
   - Make it **public**
   - Don't initialize with README

## Step 2: Push Your Files

Run these commands in Terminal:

```bash
cd "/Users/anushka/Library/Mobile Documents/com~apple~CloudDocs/website/jonbarron.github.io"

# Remove the old git remote (it points to Jon Barron's repo)
git remote remove origin

# Add your new repository (replace with your actual repo URL)
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Add all your files
git add .

# Commit your changes
git commit -m "Initial commit - Personal website"

# Push to GitHub
git push -u origin master
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in the left sidebar)
3. Under "Source", select **master** branch
4. Click **Save**
5. Your site will be live at `https://yourusername.github.io` in a few minutes!

---

## Alternative: Quick Deploy with Netlify

If you prefer, you can also:
1. Go to https://www.netlify.com/ and sign up (free)
2. Drag and drop the `jonbarron.github.io` folder onto Netlify
3. Your site will be live instantly!

