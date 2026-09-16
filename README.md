# Crypto Faucet Guide - GitHub Pages

A modern, educational website about cryptocurrency faucets with curated faucet listings and affiliate links.

## 🚀 Features

- **Modern Design**: Beautiful gradient backgrounds, smooth animations, and responsive layout
- **Educational Content**: Comprehensive information about crypto faucets and how they work
- **Curated Faucet List**: Verified faucets with affiliate links
- **Interactive Elements**: FAQ accordion, smooth scrolling, and scroll animations
- **Mobile Responsive**: Works perfectly on all devices

## 📁 Project Structure

```
crypto-earner/
├── index.html      # Main HTML file
├── styles.css      # Styling and animations
├── script.js       # Interactive JavaScript
└── README.md       # This file
```

## 🛠️ Local Development

1. Clone this repository
2. Open `index.html` in your browser, or
3. Use a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have http-server installed)
   npx http-server
   ```
4. Open `http://localhost:8000` in your browser

## 🌐 Deploying to GitHub Pages

### Option 1: Using GitHub CLI (gh)

```bash
# Initialize git if not already done
git init
git add .
git commit -m "Initial commit"

# Create repository on GitHub
gh repo create crypto-earner --public --source=.

# Enable GitHub Pages
gh api repos/:owner/:repo/pages -X PUT -f source.branch=main
```

### Option 2: Manual GitHub Setup

1. **Push to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/crypto-earner.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under **Source**, select **Deploy from a branch**
   - Select **main** branch and **/ (root)** folder
   - Click **Save**

3. **Access your site**:
   - Your site will be available at `https://YOUR_USERNAME.github.io/crypto-earner/`

### Option 3: Using Custom Domain

If you want to use a custom domain:

1. Buy a domain from a registrar (e.g., Namecheap, GoDaddy)
2. In your repository Settings → Pages, add your custom domain
3. Configure DNS records at your registrar:
   - Add a CNAME record pointing to `YOUR_USERNAME.github.io`
   - Or add A records pointing to GitHub Pages IPs

## 📝 Adding More Faucets

To add more faucets to the list, edit `index.html` and add a new faucet card in the `faucets-grid` section:

```html
<div class="faucet-card fade-in">
    <div class="faucet-header">
        <div class="faucet-icon">🎯</div>
        <div class="faucet-name">Faucet Name</div>
    </div>
    <div class="faucet-info">
        <p><strong>Type:</strong> Description</p>
        <p><strong>Timer:</strong> Claim frequency</p>
        <p><strong>Features:</strong> Any special features</p>
    </div>
    <a href="YOUR_AFFILIATE_LINK" target="_blank" class="btn btn-faucet">
        Visit Faucet
        <svg class="arrow-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <path d="M5 12h14M12 5l7 7-7 7"/>
        </svg>
    </a>
</div>
```

## 🎨 Customization

### Colors
Edit `styles.css` to change the color scheme:
```css
:root {
    --primary: #6366f1;
    --secondary: #10b981;
    --accent: #f59e0b;
    /* ... more colors */
}
```

### Fonts
Change fonts in `index.html` by modifying the Google Fonts link.

### Animations
Adjust animation speeds and effects in `styles.css` under the `@keyframes` sections.

## 🔧 Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with gradients, animations, and flexbox/grid
- **JavaScript (Vanilla)**: Interactive features and scroll animations
- **Google Fonts**: Inter font family

## 📄 License

This project is open source and available for educational purposes.

## ⚠️ Disclaimer

This website provides educational information about cryptocurrency faucets. Cryptocurrency investments carry risks. Always do your own research and never invest more than you can afford to lose.

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📧 Support

For questions or support, please open an issue on GitHub.

---

**Happy earning! 💰**
