# How to Deploy This Website

## Option 1: GitHub Pages (Recommended - Free)

### Step 1: Create a New GitHub Repository
1. Go to https://github.com/new
2. Create a repository named `yourusername.github.io` (replace `yourusername` with your GitHub username)
   - For example: `anushkadeshpande.github.io`
   - Make it **public**
   - Don't initialize with README

### Step 2: Push Your Files
```bash
cd "/Users/anushka/Library/Mobile Documents/com~apple~CloudDocs/website/jonbarron.github.io"

# Remove the old git remote (it points to Jon Barron's repo)
git remote remove origin

# Add your new repository
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Add and commit your changes
git add .
git commit -m "Initial commit - Personal website"

# Push to GitHub
git push -u origin master
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Source", select **master** branch
4. Click **Save**
5. Your site will be live at `https://yourusername.github.io` in a few minutes!

---

## Option 2: Netlify (Easy Drag & Drop - Free)

1. Go to https://www.netlify.com/ and sign up (free)
2. Drag and drop the `jonbarron.github.io` folder onto Netlify
3. Your site will be live instantly with a URL like `random-name-123.netlify.app`
4. You can add a custom domain later if you want

---

## Option 3: Vercel (Easy - Free)

1. Go to https://vercel.com/ and sign up (free)
2. Install Vercel CLI: `npm i -g vercel`
3. In the `jonbarron.github.io` folder, run: `vercel`
4. Follow the prompts
5. Your site will be live instantly

---

## Option 4: View Locally

To preview your website locally:

1. Open Terminal
2. Navigate to the folder:
   ```bash
   cd "/Users/anushka/Library/Mobile Documents/com~apple~CloudDocs/website/jonbarron.github.io"
   ```
3. Start a simple server:
   ```bash
   python3 -m http.server 8000
   ```
4. Open your browser and go to: `http://localhost:8000`

---

## Notes

- Make sure you have a profile photo at `images/profile.jpg` (or update the path in `index.html`)
- Add logos/images for universities and companies if you want (or remove those image references)
- The resume PDF is already linked at `data/resume.pdf`

