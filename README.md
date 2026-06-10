# Stackline - Professional App Website

A modern, responsive website for your mobile app with built-in download functionality.

## Features

✨ **Modern Design**
- Clean and professional layout
- Gradient backgrounds and smooth animations
- Fully responsive (mobile, tablet, desktop)
- Beautiful phone mockup on hero section

🚀 **Key Sections**
- Hero/Landing section with CTA button
- Features showcase with 6 feature cards
- Screenshot/Gallery section
- Download section with system requirements
- Statistics/KPIs display
- Contact form
- Social media links in footer

📱 **Download Integration**
- Direct APK download button
- Coming Soon placeholder for iOS
- System requirements checklist
- Pre-configured for `app-debug.apk`

⚡ **Interactive Elements**
- Smooth scrolling navigation
- Mobile hamburger menu
- Form validation
- Counter animations for statistics
- Hover effects and transitions
- Scroll-based navbar effects
- Parallax scrolling

## File Structure

```
website stackline/
├── index.html          # Main HTML file
├── styles.css          # All styling and responsive design
├── script.js           # JavaScript for interactivity
├── app-debug.apk       # Your app APK file
└── README.md           # This file
```

## How to Use

### 1. **Local Testing**
Simply open `index.html` in your web browser. No server required for basic testing.

### 2. **Customize for Your App**

#### Update App Information
Edit `index.html` and change:
- App name: Look for "Stackline" and replace with your app name
- App description: Update the subtitle and feature descriptions
- Contact info: Change email, phone, and address in the contact section
- Social media links: Update the footer social links

#### Update Styling
Edit `styles.css` to customize:
- **Colors**: Modify `:root` CSS variables at the top
  - `--primary-color`: Main brand color
  - `--secondary-color`: Secondary accent
  - `--accent-color`: CTA button color
- **Fonts**: Change `font-family` in body styles
- **Spacing**: Adjust padding/margins as needed

#### Add Screenshots
Replace the placeholder gallery items in the Screenshots section:
- Replace `.gallery-image.placeholder` divs with actual images
- Example: `<img src="screenshot1.png" alt="App screenshot">`

### 3. **Deploy to Web**
Options for hosting:
- **GitHub Pages** (Free): Push to GitHub and enable Pages
- **Netlify** (Free): Drag and drop the folder
- **Vercel** (Free): Connect your repository
- **Traditional Hosting**: Upload files via FTP

## Download Section

The APK download is already configured:
- Button points to `app-debug.apk` 
- Uses HTML5 download attribute
- Works directly when deployed

To rename or update the APK:
1. Replace `app-debug.apk` file
2. Update the `href` in the download button:
   ```html
   <a href="your-app-name.apk" class="download-btn android" download>
   ```

## Mobile Responsiveness

The site is fully responsive with breakpoints at:
- 768px (tablet)
- 480px (small phones)

Test on mobile using browser DevTools (F12 → Toggle Device Toolbar)

## Contact Form

The contact form currently shows an alert on submission. To make it functional:
1. Use a service like Formspree, EmailJS, or Netlify Forms
2. Or connect to a backend API

Example with Formspree:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="contact-form">
```

## SEO Optimization Tips

1. Update the `<title>` tag for better search results
2. Add meta description in `<head>`:
   ```html
   <meta name="description" content="Your app description here">
   ```
3. Add Open Graph tags for social media sharing
4. Optimize images (compress PNG/JPG files)

## Browser Compatibility

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

## Performance Tips

1. **Optimize Images**: Compress all images to reduce file size
2. **Lazy Loading**: Add `loading="lazy"` to images
3. **Minify CSS/JS**: Use online tools to minify files for production
4. **CDN**: Consider using a CDN for Font Awesome icons

## Customization Examples

### Change Brand Color
In `styles.css`, update:
```css
:root {
    --primary-color: #YourColorHere;
    --secondary-color: #YourColorHere;
    --accent-color: #YourColorHere;
}
```

### Add Your Logo
In `index.html`, replace the logo in navbar:
```html
<div class="nav-logo">
    <img src="your-logo.png" alt="Logo">
    Your App Name
</div>
```

### Update APK Download Link
To host APK on external storage (optional):
```html
<a href="https://your-storage.com/app.apk" class="download-btn android" download>
```

## Support & Help

For questions or issues:
- Check the code comments in each file
- Review the inline HTML structure
- Test in browser DevTools (F12)
- Validate HTML at validator.w3.org

## License

Free to use and modify for your app!

---

**Made with ❤️ for your app**
