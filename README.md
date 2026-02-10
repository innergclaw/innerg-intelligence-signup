# InnerG Intelligence | Member Signup Page

A clean, aesthetic email signup page for collecting member emails. Uses Formspree for free, no-backend form handling.

## Features

- ✅ Free email collection via Formspree (50 submissions/month free)
- ✅ Matrix rain background (matching InnerG aesthetic)
- ✅ Terminal green styling with glow effects
- ✅ Mobile responsive
- ✅ No backend required
- ✅ GitHub Pages ready

## Quick Setup (5 minutes)

### 1. Create Formspree Account

1. Go to [formspree.io](https://formspree.io/)
2. Sign up for free account
3. Click **"New Form"**
4. Enter `innerg-intel` as the form name
5. Click **"Create Form"**
6. Copy your **Form ID** (looks like: `xqkrpvnb`)

### 2. Update Form ID

Open `index.html` and replace `YOUR_FORM_ID` with your actual Formspree Form ID:

```html
<form id="signup-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

Example:
```html
<form id="signup-form" action="https://formspree.io/f/xqkrpvnb" method="POST">
```

### 3. Deploy to GitHub Pages

#### Option A: Using GitHub UI (Easiest)

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `innerg-intelligence-signup`
3. Make it **Public**
4. Click **"Create repository"**
5. Click **"uploading an existing file"**
6. Drag and drop `index.html` and `README.md`
7. Click **"Commit changes"**
8. Go to Settings → Pages
9. Source: Select **Deploy from a branch**
10. Branch: `main` → **Save**
11. Your site will be live at: `https://YOUR_USERNAME.github.io/innerg-intelligence-signup`

#### Option B: Using Git (Command Line)

```bash
# Initialize git repo
git init

# Add files
git add .

# Commit
git commit -m "Initial commit: InnerG signup page"

# Add remote (replace with your GitHub URL)
git remote add origin https://github.com/YOUR_USERNAME/innerg-intelligence-signup.git

# Push to GitHub
git branch -M main
git push -u origin main

# Then enable GitHub Pages in repo Settings
```

## Managing Emails

All collected emails will be sent to:
- Your Formspree dashboard (view anytime)
- The email address you used for your Formspree account

To send updates, you can:
1. Export emails from Formspree (CSV)
2. Use your email client or a mailing service
3. Or upgrade to Formspree Pro for built-in campaigns

## Customization

### Change Colors

Edit CSS variables in `index.html`:

```css
:root {
    --accent: #00ff41;  /* Change this for different accent color */
    --accent-glow: rgba(0, 255, 65, 0.4);  /* Match accent */
}
```

### Add More Fields

Add inputs to the form:

```html
<input type="text" name="name" placeholder="Your name">
<input type="email" name="email" placeholder="Enter your email">
```

### Change Success Message

Edit the `#success-message` div:

```html
<div id="success-message" class="success-message">
    ✓ Your custom message here
</div>
```

## Hosting Options

**GitHub Pages** (Recommended)
- ✅ Free forever
- ✅ Custom domain supported
- ✅ Auto-deploys on push

**Netlify / Vercel**
- ✅ Drag-and-drop deploy
- ✅ Free tier available
- ✅ Preview URLs for testing

## Tech Stack

- HTML5
- CSS3 (Custom, no frameworks)
- JavaScript (Vanilla, no libraries)
- Canvas API (Matrix effect)
- Formspree (Form handling)

## License

MIT — InnerG Intel

---

> "Become intelligence. Become INNERG."
