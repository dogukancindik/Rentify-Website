# Rentify Landing Page

A modern, responsive landing page for **Rentify** - a premium rent tracking application for landlords and tenants.

## 🏠 About Rentify

Rentify is a comprehensive mobile application that simplifies rent management with intelligent tracking, instant payments, and seamless communication between landlords and tenants. The app features role-based flows, real-time payment tracking, integrated payment system, and map-based location services.

## ✨ Features

- **Modern Design**: Premium aesthetic with subtle gradients, smooth shadows, and micro-interactions
- **Dark Mode**: Fully functional light/dark theme toggle with localStorage persistence
- **Responsive**: Optimized for mobile, tablet, and desktop devices
- **Interactive Gallery**: Category-based filtering with lightbox modal and keyboard navigation
- **Smooth Animations**: Polished transitions and hover effects throughout
- **Performance Optimized**: Lazy loading images, debounced scroll events, minimal JavaScript
- **Accessible**: Proper focus styles, semantic HTML, and reduced motion support
- **SEO Ready**: Meta tags, Open Graph tags, and semantic structure

## 📁 Project Structure

```
rentify-landing/
├── index.html                 # Main HTML file
├── README.md                  # This file
├── assets/
│   ├── css/
│   │   └── style.css         # All styles with CSS variables
│   ├── js/
│   │   └── main.js           # Interactive functionality
│   └── images/
│       └── screenshots/      # App screenshots (10 images)
│           ├── Screenshot_1767274392.png
│           ├── Screenshot_1767274404.png
│           ├── Screenshot_1767274425.png
│           ├── Screenshot_1767274429.png
│           ├── Screenshot_1767274452.png
│           ├── Screenshot_1767274461.png
│           ├── Screenshot_1767274485.png
│           ├── Screenshot_1767274489.png
│           ├── Screenshot_1767274501.png
│           └── Screenshot_1767274508.png
```

## 🚀 Running Locally

### Option 1: Direct File Open
Simply open `index.html` in your web browser:
```bash
open index.html
# or double-click the file in your file explorer
```

### Option 2: Local Web Server (Recommended)
Using a local server prevents CORS issues and simulates production environment:

**Using Python 3:**
```bash
cd rentify-landing
python3 -m http.server 8000
# Visit http://localhost:8000
```

**Using Node.js (npx):**
```bash
cd rentify-landing
npx -y http-server -p 8000
# Visit http://localhost:8000
```

**Using PHP:**
```bash
cd rentify-landing
php -S localhost:8000
# Visit http://localhost:8000
```

## 🌐 GitHub Pages Deployment

Follow these steps to publish your landing page on GitHub Pages:

### 1. Create a GitHub Repository
```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit your changes
git commit -m "Initial commit: Rentify landing page"

# Create a new repository on GitHub, then:
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

### 2. Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on **Settings** (gear icon)
3. Scroll down to **Pages** section in the left sidebar
4. Under **Source**, select:
   - **Branch**: `main`
   - **Folder**: `/ (root)` or `/rentify-landing` (depending on your structure)
5. Click **Save**

### 3. Access Your Site
After a few minutes, your site will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

If you placed files in a `rentify-landing` subdirectory:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/rentify-landing/
```

### 4. Custom Domain (Optional)
To use a custom domain:
1. Add a `CNAME` file to your repository root with your domain name
2. Configure DNS settings with your domain provider
3. Update the custom domain in GitHub Pages settings

## 📸 Screenshots Setup

The landing page expects 10 app screenshots in `assets/images/screenshots/` with these exact filenames:
- `Screenshot_1767274392.png` - Auth: Sign In
- `Screenshot_1767274404.png` - Roles: Role Selection  
- `Screenshot_1767274425.png` - Apartments: My Apartments
- `Screenshot_1767274429.png` - Apartments: Invite Tenant
- `Screenshot_1767274452.png` - Profile/Map: Profile Screen
- `Screenshot_1767274461.png` - Profile/Map: Map Location
- `Screenshot_1767274485.png` - Profile/Map: Profile Details
- `Screenshot_1767274489.png` - Requests: Requests Screen
- `Screenshot_1767274501.png` - Mini Bank: Payment Receipt
- `Screenshot_1767274508.png` - Mini Bank: Payment Success

These images are categorized in the gallery as:
- **Auth**: Sign-in screens
- **Roles**: Role selection
- **Apartments**: Property management and tenant invitations
- **Profile/Map**: User profile and location picker
- **Requests**: Tenant request management
- **Mini Bank**: Payment system and receipts

To optimize images for web:
```bash
# Using ImageMagick (install via: brew install imagemagick)
mogrify -resize 1080x -quality 85 assets/screenshots/*.jpeg
```

## 🎨 Customization

### Colors
Edit CSS variables in `assets/css/style.css`:
```css
:root {
    --primary: #6366f1;
    --secondary: #ec4899;
    --accent: #14b8a6;
    /* ... more variables */
}
```

### Content
Edit text directly in `index.html`:
- Hero section: Update tagline, description, and CTA links
- Features: Modify feature cards
- FAQ: Add/remove questions
- Footer: Update links and information

### Call-to-Action Buttons
Update the `href` attributes in the hero section:
```html
<a href="mailto:your-email@rentify.app?subject=Demo Request" class="btn btn-primary btn-lg">Request Demo</a>
<a href="https://github.com/your-username/your-repo" class="btn btn-secondary btn-lg">View on GitHub</a>
```

## 🛠️ Technologies Used

- **HTML5**: Semantic structure
- **CSS3**: Modern styling with CSS Grid, Flexbox, and CSS Variables
- **Vanilla JavaScript**: No frameworks or dependencies
- **LocalStorage**: Theme preference persistence
- **Intersection Observer API**: Lazy loading images

## 📱 Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

---
