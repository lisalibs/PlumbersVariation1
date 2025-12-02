# ABC Plumbing Website Template

A modern, responsive, and SEO-optimized website template designed for plumbing businesses. This template features a professional design, accessibility best practices, and Schema.org structured data for better search engine visibility.

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Features

- **Fully Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Accessibility First** - WCAG compliant with ARIA labels, skip links, and keyboard navigation
- **SEO Optimized** - Includes meta tags, Open Graph, Twitter Cards, and Schema.org structured data
- **Modern UI/UX** - Clean, professional design with smooth animations and transitions
- **Easy Customization** - Well-documented CSS variables for quick color and style changes
- **Contact Form** - Built-in form validation (backend integration required)
- **Mobile Menu** - Touch-friendly navigation with focus trapping
- **24/7 Availability Badge** - Highlights emergency services
- **Customer Testimonials** - Social proof section
- **Service Area Display** - Clearly shows coverage areas

## Sections Included

1. **Header** - Fixed navigation with logo and phone number
2. **Hero Section** - Eye-catching intro with call-to-action buttons
3. **Trust Bar** - Key benefits and certifications
4. **Services** - 6 service cards showcasing offerings
5. **Why Choose Us** - Features and benefits section
6. **Testimonials** - Customer reviews and ratings
7. **Service Area** - Geographic coverage display
8. **Call-to-Action** - Prominent contact section
9. **Contact Form** - Quote request form with validation
10. **Footer** - Company info and links

## Quick Start

1. **Clone or Download** the repository
2. **Open `index.html`** in your browser
3. **Customize** the content (see Customization section below)
4. **Deploy** to your web hosting

No build process or dependencies required - just open and edit!

## Customization Guide

### 1. Colors

Edit the CSS variables in the `<style>` section (lines 25-34):

```css
:root {
    /* PRIMARY COLORS - Edit these for each client */
    --primary: #0c4a6e;        /* Deep blue - main brand color */
    --primary-light: #0369a1;  /* Lighter blue for hover states */
    --primary-dark: #082f49;   /* Darker blue for depth */

    /* ACCENT COLOR - The pop of color */
    --accent: #f59e0b;         /* Warm amber/orange */
    --accent-light: #fbbf24;
    --accent-dark: #d97706;
}
```

### 2. Business Information

Replace all instances of:
- **Company Name**: "ABC Plumbing" (appears throughout)
- **Phone Number**: "(519) 555-1234" or "+15195551234"
- **Email**: "info@abcplumbing.com"
- **Address**: "123 Main Street, Chatham, ON N7M 1A1"

### 3. Services

Edit the services section (starting at line 1377) to match your offerings.

### 4. Testimonials

Update testimonials (starting at line 1527) with real customer reviews.

### 5. Service Areas

Modify the areas list (starting at line 1593) to match your coverage area.

### 6. Meta Tags & SEO

Update meta tags in the `<head>` section:
- Meta description (line 6)
- Open Graph tags (lines 10-16)
- Twitter Card tags (lines 18-22)
- Schema.org data (lines 1214-1273)

### 7. Logo

Replace the placeholder SVG icon with your actual logo:
- Header logo (lines 1183-1189)
- Footer logo (lines 1736-1742)

### 8. Images

Update image URLs:
- Open Graph image: `og-image.jpg` (1200x630px recommended)
- Favicon files: `favicon-32x32.png`, `favicon-16x16.png`, `apple-touch-icon.png`

## File Structure

```
plumbers/
├── index.html          # Main website file
├── README.md          # This file
├── LICENSE            # MIT License
└── .gitignore        # Git ignore rules
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Accessibility Features

- Skip to main content link
- ARIA labels and roles
- Keyboard navigation support
- Focus trapping in mobile menu
- Semantic HTML structure
- Sufficient color contrast ratios
- Screen reader friendly

## SEO Features

- Meta description and keywords
- Open Graph tags for social sharing
- Twitter Card support
- Schema.org LocalBusiness structured data
- Semantic HTML5 elements
- Proper heading hierarchy
- Mobile-friendly design

## Form Integration ⚡

**The form is pre-configured for Formspree!** See [FORMSPREE-SETUP.md](FORMSPREE-SETUP.md) for complete instructions.

### Quick Setup (5 minutes):
1. Sign up at https://formspree.io with your email
2. Create a form and get your Form ID
3. Replace `YOUR_FORM_ID` in line 1765 of index.html
4. Done! Form submissions will go to your email

### Alternative Options

If you prefer a different solution:

1. Replace the form submission handler (line 1901-1948)
2. Add your API endpoint
3. Implement server-side validation
4. Set up email notifications or CRM integration

Example using fetch API:

```javascript
fetch('/api/contact', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ name, phone, email, service, message })
})
.then(response => response.json())
.then(data => {
    alert('Thank you! We\'ll contact you soon.');
    form.reset();
})
.catch(error => {
    alert('Sorry, something went wrong. Please call us directly.');
});
```

## Performance Optimization

Current setup:
- CSS and JavaScript are inline for simplicity
- Google Fonts loaded from CDN
- Minimal external dependencies

For production:
1. Consider self-hosting fonts
2. Minify CSS and JavaScript
3. Optimize and compress images
4. Enable gzip/brotli compression on server
5. Set up proper caching headers

## Deployment

### Static Hosting (GitHub Pages, Netlify, Vercel)

1. Push to GitHub repository
2. Connect to hosting platform
3. Deploy from main branch

### Traditional Web Hosting

1. Upload `index.html` and assets via FTP
2. Point domain to hosting directory
3. Ensure SSL certificate is installed

## Support

For issues, questions, or suggestions:
- Open an issue in the repository
- Check existing documentation
- Review the customization guide

## Credits

- **Fonts**: Plus Jakarta Sans & DM Serif Display (Google Fonts)
- **Icons**: Custom SVG icons
- **Design**: Modern, professional plumbing industry design

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Changelog

### Version 1.0.0 (2024-12-02)
- Initial release
- Fully responsive design
- Accessibility improvements
- SEO optimization
- Schema.org structured data
- Form validation
- Mobile menu with focus trapping

---

**Built with care for small business owners.** 💙

For customization help or web development services, contact your web developer.
