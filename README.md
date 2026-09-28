# Vineet Chaudhary - Portfolio Website

A modern, responsive portfolio website built with HTML5, CSS3, and vanilla JavaScript. This portfolio showcases skills, projects, and contact information in a professional dark theme with smooth animations.

## 🚀 Quick Start with VS Code Live Server

### Step 1: Install VS Code
If you don't have VS Code installed, download it from: https://code.visualstudio.com/

### Step 2: Install Live Server Extension
1. Open VS Code
2. Click on the Extensions icon in the left sidebar (or press `Ctrl+Shift+X`)
3. Search for "Live Server"
4. Install the "Live Server" extension by Ritwick Dey

### Step 3: Open the Project
1. Open VS Code
2. Click "File" → "Open Folder"
3. Navigate to and select the `portfolio` folder
4. Click "Select Folder"

### Step 4: Run with Live Server
1. Right-click on `index.html` in the file explorer
2. Select "Open with Live Server"
3. The website will automatically open in your default browser

**Alternative Method:**
- Click "Go Live" in the bottom right corner of VS Code

### Step 5: Development
- Any changes you make to HTML, CSS, or JavaScript files will automatically reload in the browser
- No need to manually refresh the page

## 📁 Project Structure

```
portfolio/
│
├── index.html          # Main HTML file with all sections
├── style.css           # Custom CSS with modern dark theme
├── script.js           # JavaScript for interactions and animations
├── README.md           # This file
└── assets/
    ├── README.md       # Instructions for assets
    └── profile.jpg     # Your profile photo (add this)
```

## 🎨 Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Modern Dark Theme**: Professional dark theme with blue/purple accents
- **Smooth Animations**: Scroll reveal, typing effect, and hover animations
- **Glassmorphism**: Modern glass-like card effects
- **Interactive Elements**: Working navigation, form validation, and buttons
- **Performance Optimized**: Debounced scroll events and lazy loading
- **Accessible**: Semantic HTML and ARIA labels
- **SEO Friendly**: Proper meta tags and structure

## 📝 Sections Included

1. **Navbar**: Sticky navigation with smooth scrolling and mobile menu
2. **Hero Section**: Introduction with typing animation and social links
3. **About Section**: Personal information with info cards
4. **Skills Section**: Interactive skill cards with progress bars
5. **Projects Section**: Project cards with images and links
6. **Education Section**: Timeline of education
7. **Why Hire Me**: Feature cards highlighting strengths
8. **Contact Section**: Working contact form with validation
9. **Footer**: Copyright and social media links

## 🔧 Customization Guide

### 1. Replace Profile Photo
**Location**: `assets/profile.jpg`

1. Prepare your profile photo (recommended: 400x400px, square format)
2. Rename it to `profile.jpg`
3. Place it in the `assets` folder
4. The website will automatically load it

**If you don't have a photo yet**: The website will still work, but the image area will be empty.

### 2. Update Personal Information

#### GitHub Username
**File**: `index.html`
**Search for**: `yourusername`
**Replace with**: Your actual GitHub username

**Locations in index.html:**
- Line ~125: Hero section GitHub link
- Line ~247: Project 1 GitHub link
- Line ~271: Project 2 GitHub link
- Line ~295: Project 3 GitHub link
- Line ~355: Contact section GitHub
- Line ~388: Footer GitHub

**Example:**
```html
<!-- Before -->
<a href="https://github.com/yourusername" target="_blank">

<!-- After -->
<a href="https://github.com/vineetchaudhary" target="_blank">
```

#### LinkedIn Username
**File**: `index.html`
**Search for**: `yourusername`
**Replace with**: Your actual LinkedIn username

**Locations in index.html:**
- Line ~128: Hero section LinkedIn link
- Line ~358: Contact section LinkedIn
- Line ~391: Footer LinkedIn

**Example:**
```html
<!-- Before -->
<a href="https://linkedin.com/in/yourusername" target="_blank">

<!-- After -->
<a href="https://linkedin.com/in/vineet-chaudhary" target="_blank">
```

#### Email Address
**File**: `index.html`
**Search for**: `your.email@example.com`
**Replace with**: Your actual email address

**Locations in index.html:**
- Line ~352: Contact section email
- Line ~394: Footer email

**Example:**
```html
<!-- Before -->
<p>your.email@example.com</p>

<!-- After -->
<p>vineet.chaudhary@example.com</p>
```

### 3. Update Project Links

#### Project Live Demo Links
**File**: `index.html`
**Search for**: `href="#"` in project sections
**Replace with**: Your actual project URLs

**Locations:**
- Line ~250: Project 1 Live Demo
- Line ~274: Project 2 Live Demo
- Line ~298: Project 3 Live Demo

**Example:**
```html
<!-- Before -->
<a href="#" target="_blank" class="btn btn-primary">

<!-- After -->
<a href="https://your-project-demo.com" target="_blank" class="btn btn-primary">
```

#### Project Images
**File**: `index.html`
**Search for**: `via.placeholder.com`
**Replace with**: Your actual project screenshot URLs

**Locations:**
- Line ~243: Project 1 image
- Line ~267: Project 2 image
- Line ~291: Project 3 image

**Example:**
```html
<!-- Before -->
<img src="https://via.placeholder.com/400x250/1a1a2e/6366f1?text=Library+Management" alt="...">

<!-- After -->
<img src="assets/library-project.jpg" alt="...">
```

### 4. Update Skill Percentages
**File**: `index.html`
**Search for**: `data-progress`
**Replace with**: Your actual skill levels (0-100)

**Example:**
```html
<!-- Before -->
<div class="skill-progress" data-progress="85"></div>

<!-- After -->
<div class="skill-progress" data-progress="90"></div>
```

### 5. Customize Colors (Optional)
**File**: `style.css`
**Lines**: 8-17 (CSS Variables)

```css
:root {
    --primary-color: #6366f1;      /* Main accent color */
    --secondary-color: #8b5cf6;    /* Secondary accent color */
    --accent-color: #10b981;       /* Success/green color */
    --dark-bg: #0f0f1a;            /* Background color */
    --card-bg: rgba(255, 255, 255, 0.05);  /* Card background */
    --text-primary: #ffffff;       /* Main text color */
    --text-secondary: #a0a0a0;     /* Secondary text color */
    --gradient: linear-gradient(135deg, #6366f1, #8b5cf6);  /* Gradient */
}
```

### 6. Update Typing Animation Roles
**File**: `script.js`
**Line**: 13

```javascript
// Before
const roles = ['Software Engineer', 'B.Tech CSE Student', 'Java DSA Developer', 'Web Developer'];

// After (customize as needed)
const roles = ['Software Engineer', 'Full Stack Developer', 'Java Developer', 'Web Developer'];
```

## 🎯 How to Make the Contact Form Work

Currently, the contact form shows a success message but doesn't actually send emails. To make it functional:

### Option 1: Use Formspree (Easiest)
1. Sign up at https://formspree.io/
2. Create a new form
3. Get your form endpoint URL
4. Update the form in `index.html`:

```html
<form id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: Use EmailJS
1. Sign up at https://www.emailjs.com/
2. Follow their documentation to integrate
3. Update the JavaScript in `script.js` to use EmailJS API

### Option 3: Backend Integration
For a production website, you'll need a backend service to handle form submissions.

## 📱 Testing Responsiveness

1. Open the website in your browser
2. Press `F12` to open Developer Tools
3. Click the device toggle icon (or press `Ctrl+Shift+M`)
4. Test different device sizes:
   - Mobile: 375x667 (iPhone SE)
   - Tablet: 768x1024 (iPad)
   - Desktop: 1920x1080

## 🐛 Troubleshooting

### Website doesn't load
- Make sure you're using Live Server, not just opening the HTML file
- Check that all files (index.html, style.css, script.js) are in the same folder

### Images not showing
- Verify your profile photo is named `profile.jpg` and in the `assets` folder
- Check file paths in HTML are correct

### Mobile menu not working
- Ensure `script.js` is properly linked in `index.html`
- Check browser console for JavaScript errors (Press `F12` → Console)

### Animations not smooth
- Disable browser extensions that might interfere
- Check if your browser supports CSS animations

### Styling looks wrong
- Clear browser cache
- Ensure `style.css` is properly linked
- Check for CSS syntax errors in browser console

## 🌐 Deployment

### Free Hosting Options:

1. **GitHub Pages** (Recommended)
   - Create a GitHub repository
   - Upload your files
   - Enable GitHub Pages in repository settings
   - Your site will be live at `yourusername.github.io/portfolio`

2. **Netlify**
   - Drag and drop your portfolio folder to https://app.netlify.com/drop
   - Instant deployment with free SSL

3. **Vercel**
   - Similar to Netlify, drag and drop deployment
   - Visit https://vercel.com/

## 📊 Browser Compatibility

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🔒 Security Notes

- Remove any sensitive information before deploying
- Update placeholder links with real URLs
- Consider adding a robots.txt file
- Add a sitemap.xml for better SEO

## 📝 License

This portfolio template is free to use and modify for personal and commercial purposes.

## 🤝 Support

If you encounter any issues:
1. Check the troubleshooting section above
2. Verify all file paths are correct
3. Check browser console for errors (F12)
4. Ensure you're using a modern browser

---

**Built with ❤️ using HTML, CSS, and JavaScript**
**No frameworks, no dependencies, just clean code**
