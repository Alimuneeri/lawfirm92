# Lexbridge Solicitors - Jekyll Website

A professional, responsive Jekyll website for a premier Indian law firm featuring modern design, smooth animations, and comprehensive practice area coverage.

## Features

- **Responsive Design**: Mobile-first approach with Bootstrap 5
- **Modern Animations**: Smooth transitions and scroll effects
- **SEO Optimized**: Jekyll SEO plugin integration
- **Blog System**: Built-in blog with categories and tags
- **Contact Forms**: Professional contact forms with validation
- **Social Integration**: Social media links and sharing

## Practice Areas

- General Corporate
- Private Equity
- Banking & Finance
- Insolvency & Restructuring
- Competition Law
- Dispute Resolution
- Infrastructure, Energy and Project Finance
- Capital Markets
- Tax
- Intellectual Property

## Installation

1. **Clone the repository**
   ```bash
   git clone [your-repo-url]
   cd extracted-directory
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run the development server**
   ```bash
   bundle exec jekyll serve
   ```

4. **Visit your site**
   Open `http://localhost:4000` in your browser

## Configuration

### Site Settings
Edit `_config.yml` to update:
- Site title and description
- Contact information
- Social media links
- SEO settings

### Content Management

#### Team Members
Update team information in `_data/team.yml`:
```yaml
- name: "Lawyer Name"
  position: "Title"
  specialization: "Practice Area"
  experience: "Years"
  bio: "Biography"
  email: "email@domain.com"
  image: "/assets/img/team/photo.jpg"
```

#### Services
Modify practice areas in `_data/services.yml`:
```yaml
- title: "Service Name"
  description: "Service description"
  icon: "fas fa-icon-name"
```

#### Awards
Update recognition in `_data/awards.yml`:
```yaml
- title: "Award Title"
  organization: "Awarding Body"
  year: "Year"
  description: "Description"
  logo: "/assets/img/awards/logo.png"
```

#### Testimonials
Add client feedback in `_data/testimonials.yml`:
```yaml
- text: "Testimonial text"
  author: "Client Name"
  position: "Title"
  company: "Company Name"
```

### Blog Posts

Create new blog posts in `_posts/` directory:
```yaml
---
layout: post
title: "Post Title"
date: YYYY-MM-DD
author: "Author Name"
category: "Category"
tags: ["tag1", "tag2"]
excerpt: "Post excerpt"
---

Post content here...
```

### Styling

Custom styles are in `assets/css/style.css`. The CSS uses:
- CSS custom properties for easy theme customization
- Bootstrap 5 for responsive grid and components
- Font Awesome for icons
- Google Fonts (Inter) for typography

#### Color Scheme
```css
:root {
    --primary-color: #1e3a8a;    /* Navy blue */
    --secondary-color: #f59e0b;   /* Gold */
    --accent-color: #10b981;      /* Green */
}
```

## Deployment

### GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Site will be available at `https://username.github.io/repository-name`

### Netlify
1. Connect repository to Netlify
2. Set build command: `bundle exec jekyll build`
3. Set publish directory: `_site`

### Other Hosting
1. Run `bundle exec jekyll build`
2. Upload `_site` directory contents to web server

## Customization

### Adding New Sections
1. Create include file in `_includes/new-section.html`
2. Add to `index.html`: `{% include new-section.html %}`
3. Add navigation link in `_includes/navbar.html`
4. Add corresponding styles in `assets/css/style.css`

### Contact Form Integration
Replace the form action in `_includes/contact.html`:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

Options:
- **Formspree**: Easy form handling service
- **Netlify Forms**: Built-in form processing
- **Custom Backend**: Your own form processing

### Analytics
Add Google Analytics to `_config.yml`:
```yaml
google_analytics: "UA-XXXXXXXXX-X"
```

## File Structure

```
Lexbridge-Solicitors/
├── _config.yml              # Site configuration
├── Gemfile                  # Ruby dependencies
├── index.html               # Homepage
├── _layouts/                # Page templates
│   ├── default.html
│   └── post.html
├── _includes/               # Reusable components
│   ├── navbar.html
│   ├── hero.html
│   ├── services.html
│   ├── team.html
│   ├── awards.html
│   ├── blogs.html
│   ├── news.html
│   ├── testimonials.html
│   ├── podcasts.html
│   ├── contact.html
│   └── footer.html
├── _data/                   # Site data files
│   ├── services.yml
│   ├── team.yml
│   ├── awards.yml
│   ├── testimonials.yml
│   └── contact.yml
├── _posts/                  # Blog posts
├── assets/                  # Static assets
│   ├── css/
│   ├── js/
│   └── img/
└── README.md
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Performance

The site is optimized for:
- Fast loading times
- Mobile performance
- SEO best practices
- Accessibility standards

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and customization services, contact:
- Email: info@lexbridgesolicitors.com
- Phone: +91-124-4567890

---

Built with ❤️ using Jekyll and Bootstrap