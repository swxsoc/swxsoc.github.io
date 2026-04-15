# Previewing the Website Locally

This guide shows you how to preview the modernized website design before it's deployed.

## Method 1: Quick Preview with Jekyll (Recommended)

### Prerequisites
- Ruby 2.5 or higher
- Bundler

### Steps

1. **Install Jekyll and dependencies:**
   ```bash
   gem install bundler jekyll
   gem install jekyll-theme-tactile
   gem install jekyll-seo-tag
   ```

2. **Navigate to the repository:**
   ```bash
   cd /path/to/swxsoc.github.io
   ```

3. **Serve the site locally:**
   ```bash
   jekyll serve
   ```

4. **View in your browser:**
   Open [http://localhost:4000](http://localhost:4000)

The site will automatically reload when you make changes to the files.

## Method 2: Simple HTTP Server (No Jekyll Required)

If you want to preview the static files without Jekyll:

1. **Build the site (one-time):**
   ```bash
   jekyll build
   ```

2. **Serve the `_site` folder:**
   ```bash
   cd _site
   python3 -m http.server 8000
   ```

3. **View in your browser:**
   Open [http://localhost:8000](http://localhost:8000)

## Method 3: Using Docker (Easiest for consistency)

1. **Run Jekyll in Docker:**
   ```bash
   docker run --rm -it \
     -p 4000:4000 \
     -v "$PWD":/srv/jekyll \
     jekyll/jekyll:latest \
     jekyll serve
   ```

2. **View in your browser:**
   Open [http://localhost:4000](http://localhost:4000)

## What You'll See

The modernized design includes:

- **Modern color scheme** with blue theme (#2563eb)
- **Improved typography** with better fonts and spacing
- **Gradient buttons** with hover effects
- **Custom arrow bullets** (→) in lists with animations
- **Hero card** styling for the intro paragraph
- **Section dividers** with accent bars
- **Smooth animations** throughout
- **Mobile-responsive** design

## Troubleshooting

### "Command not found: jekyll"
Make sure Ruby gems are in your PATH:
```bash
export PATH="$HOME/.gem/ruby/X.X.0/bin:$PATH"
```

### Theme not found
Install the Tactile theme:
```bash
gem install jekyll-theme-tactile
```

### Port already in use
Use a different port:
```bash
jekyll serve --port 4001
```

## Viewing Changes in This PR

This PR branch (`copilot/make-site-look-modern`) includes:
- New custom CSS file: `assets/css/custom.css`
- Updated template: `_includes/head-custom.html`
- Improved content: `index.md`

All changes are purely cosmetic and don't affect functionality.
