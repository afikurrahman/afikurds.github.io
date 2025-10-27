# AIFahim Portfolio Website

A professional portfolio website built with HTML, CSS, JavaScript, and Bootstrap, showcasing my experience as a Machine Learning Engineer, research publications, projects, and achievements.

## 🌐 Live Website
Visit: [https://aifahim.github.io](https://aifahim.github.io)

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Development Setup](#development-setup)
- [Deployment](#deployment)
- [Content Management](#content-management)
- [Customization Guide](#customization-guide)
- [Contributing](#contributing)
- [Troubleshooting](#troubleshooting)

## 🎯 Overview

This portfolio website is designed to showcase:
- Professional experience and work history
- Research publications with visual gallery
- Technical projects with filtering capabilities
- Skills and expertise
- Awards and achievements
- Educational background
- Contact information

## ✨ Features

### Core Features
- **Responsive Design**: Mobile-first approach, works seamlessly on all devices
- **Smooth Scrolling Navigation**: Easy navigation with animated scroll spy
- **Project Filtering**: Isotope.js powered project gallery with category filters
- **Research Gallery**: Visual presentation of research papers with images
- **Dynamic Content**: Easy to update and maintain content structure
- **Performance Optimized**: Minified CSS/JS and optimized loading

### Technical Features
- Bootstrap 4 framework for responsive layout
- jQuery for DOM manipulation and animations
- Isotope.js for project filtering and layout
- Font Awesome and Devicons for icons
- Google Fonts for typography
- GitHub Actions for automated deployment

## 📁 Project Structure

```
aifahim.github.io/
├── .github/
│   └── workflows/
│       ├── static.yml          # GitHub Pages deployment workflow
│       └── jekyll-docker.yml   # Jekyll build workflow
├── assets/
│   ├── css/                    # Additional stylesheets
│   ├── img/
│   │   └── research/          # Research publication images
│   │       ├── covid.png
│   │       ├── dolg.png
│   │       └── ovarian.jpg.png
│   ├── js/                    # JavaScript files
│   └── fonts/                 # Custom fonts
├── css/
│   ├── resume.css             # Main stylesheet
│   └── resume.min.css         # Minified version
├── img/
│   ├── fahim.png              # Profile picture
│   └── fahim_in.jpeg          # Alternative profile
├── js/
│   ├── resume.js              # Main JavaScript
│   └── resume.min.js          # Minified version
├── vendor/                    # Third-party libraries
│   ├── bootstrap/
│   ├── jquery/
│   ├── jquery-easing/
│   ├── font-awesome/
│   ├── devicons/
│   └── simple-line-icons/
├── index.html                 # Main HTML file
├── package.json               # Node.js dependencies
└── README.md                  # This file
```

## 🛠 Technologies Used

### Frontend
- **HTML5**: Semantic markup
- **CSS3**: Custom styles with responsive design
- **JavaScript/jQuery**: Interactive features and animations
- **Bootstrap 4.3.1**: Responsive grid system and components

### Libraries & Frameworks
- **Isotope.js**: For project filtering and masonry layout
- **jQuery Easing**: Smooth scroll animations
- **Font Awesome 5.15.2**: Icon library
- **Devicons**: Developer technology icons
- **Google Fonts**: Saira Extra Condensed & Open Sans

### Development Tools
- **npm**: Package management
- **GitHub Actions**: CI/CD for deployment
- **Git**: Version control

## 💻 Development Setup

### Prerequisites
- Git installed on your machine
- A code editor (VS Code recommended)
- Basic knowledge of HTML, CSS, and JavaScript
- (Optional) Node.js and npm for package management

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/AIFahim/aifahim.github.io.git
   cd aifahim.github.io
   ```

2. **Open in browser**
   - Simply open `index.html` in your web browser
   - Or use a local server (recommended):
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js
     npx http-server
     ```

3. **Make changes**
   - Edit `index.html` for content changes
   - Modify CSS in `css/resume.css`
   - Update JavaScript in `js/resume.js`

### Development Tips
- Use browser developer tools for debugging
- Test responsive design at different breakpoints
- Validate HTML/CSS for best practices
- Check console for JavaScript errors

## 🚀 Deployment

### GitHub Pages Deployment

The website is automatically deployed using GitHub Actions when you push to the `master` branch.

1. **Commit your changes**
   ```bash
   git add .
   git commit -m "Update portfolio content"
   ```

2. **Push to GitHub**
   ```bash
   git push origin master
   ```

3. **Automatic deployment**
   - GitHub Actions will trigger automatically
   - Check Actions tab for deployment status
   - Website updates within 2-5 minutes

### Manual Deployment

If you need to deploy manually:

1. Go to repository Settings
2. Navigate to Pages section
3. Source: Deploy from branch
4. Branch: master, folder: / (root)
5. Save and wait for deployment

## 📝 Content Management

### Updating Personal Information

**Profile Section** (Lines ~500-550):
```html
<h1 class="mb-0">Md. Asif Iqbal
  <span class="text-primary">Fahim</span>
</h1>
<div class="subheading mb-5">
  Contact: <a href="mailto:asif.iqbal.ece.ruet@gmail.com">email</a>
</div>
```

### Adding Work Experience

**Experience Section** (Lines ~600-800):
```html
<div class="resume-item d-flex flex-column flex-md-row mb-5">
  <div class="resume-content mr-auto">
    <h3 class="mb-0">Position Title</h3>
    <div class="subheading mb-3">Company Name</div>
    <p>Job description here...</p>
  </div>
  <div class="resume-date text-md-right">
    <span class="text-primary">Start Date - End Date</span>
  </div>
</div>
```

### Adding Projects

**Projects Section** (Lines ~1200-1500):
```html
<li class="project-item isotope-item ml">
  <span class="project-title">
    <i class="fa-li fa fa-files-o pub-icon"></i>
    <b>Project Name</b>
  </span>
  <p class="project-summary">
    Project description here...
    <a href="link-to-project">Project Link</a>
  </p>
</li>
```

### Adding Research Publications

**Research Section** (Lines ~1750-1850):
```html
<div class="research-item">
  <div class="research-content">
    <div class="research-title">Paper Title</div>
    <div class="research-authors">Authors</div>
    <div class="research-venue">Conference/Journal</div>
    <div class="research-links">
      <a href="paper-link">Access Publication</a>
    </div>
  </div>
  <div class="research-image">
    <img src="assets/img/research/image.png" alt="Description">
  </div>
</div>
```

### Updating Skills

**Skills Section** (Lines ~1900-2000):
```html
<!-- Programming Languages -->
<li class="list-inline-item">
  <i class="devicons devicons-python"></i>
</li>

<!-- Frameworks -->
<div class="subheading mb-3">Technical Skills</div>
<ul class="fa-ul mb-0">
  <li><i class="fa-li fa fa-check"></i>
    Skill name here
  </li>
</ul>
```

## 🎨 Customization Guide

### Color Scheme

Main colors defined in CSS:
- Primary: `#BD5D38` (Orange-red)
- Text: `#868e96` (Gray)
- Headers: `#343a40` (Dark gray)

To change colors, update in `css/resume.css`:
```css
.text-primary {
  color: #BD5D38 !important;
}

.bg-primary {
  background-color: #BD5D38 !important;
}
```

### Fonts

Currently using:
- Headers: 'Saira Extra Condensed'
- Body: 'Open Sans'

To change fonts, update in `index.html`:
```html
<link href="https://fonts.googleapis.com/css?family=Your+Font" rel="stylesheet">
```

### Responsive Breakpoints

Mobile responsiveness styles (Lines ~110-180):
```css
@media (max-width: 768px) {
  /* Tablet and mobile styles */
}

@media (max-width: 576px) {
  /* Mobile only styles */
}
```

### Adding New Sections

1. Add navigation link:
```html
<li class="nav-item">
  <a class="nav-link js-scroll-trigger" href="#newsection">New Section</a>
</li>
```

2. Create section:
```html
<section class="resume-section p-3 p-lg-5 d-flex flex-column" id="newsection">
  <div class="my-auto">
    <h2 class="mb-5">New Section</h2>
    <!-- Content here -->
  </div>
</section>
```

## 🔧 Troubleshooting

### Common Issues

**GitHub Pages not updating**
- Check Actions tab for errors
- Ensure changes are pushed to master branch
- Clear browser cache

**Images not loading**
- Verify image paths are correct
- Check file extensions match exactly
- Ensure images are committed to repository

**JavaScript errors**
- Check browser console for specific errors
- Verify jQuery is loaded before other scripts
- Check for syntax errors in custom code

**Responsive issues**
- Test using browser developer tools
- Check media query breakpoints
- Verify Bootstrap classes are correct

### Performance Optimization

1. **Minimize file sizes**:
   - Use minified CSS/JS in production
   - Optimize images (use WebP format)
   - Enable browser caching

2. **Reduce HTTP requests**:
   - Combine CSS files
   - Use CSS sprites for icons
   - Lazy load images

3. **Code optimization**:
   - Remove unused CSS/JS
   - Use CDN for libraries
   - Enable GZIP compression

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Last Updated**: January 2025
**Maintained By**: Md. Asif Iqbal Fahim