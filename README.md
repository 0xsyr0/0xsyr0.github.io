# syro - Personal Blog & Portfolio

A dark-themed minimalistic static site for cybersecurity professionals, built for GitHub Pages.

## Features

- Purple cyberpunk aesthetic with dark background
- Zero dependencies - pure HTML/CSS
- Fully responsive design
- GitHub Pages ready
- Easy blog management
- Portfolio section for projects
- Social media integration

## Quick Start

1. Clone/download this repository to your GitHub Pages repo (`yourusername.github.io`)

2. Edit social links in `index.html`:
   - Update the URLs in the "Social" section with your profiles
   - Replace placeholder links with your actual profile URLs

3. Customize content:
   - Edit the "About" section with your background
   - Update projects in the Projects section
   - Modify the hero tagline

4. Push to GitHub:
   ```bash
   git add .
   git commit -m "Deploy new site"
   git push origin main
   ```

5. Your site will be live at `https://yourusername.github.io`

## Adding Blog Posts

### Creating a New Post

1. Copy `posts/post-1.html` to create a new post:
   ```bash
   cp posts/post-1.html posts/your-new-post.html
   ```

2. Edit the new post file:
   - Change the `<title>` and `<h1>` tags
   - Update the date and tags
   - Write your content in the `.post-content` section

3. Add the post to the blog grid in `index.html`:
   ```html
   <article class="blog-card">
       <span class="blog-date">2024-02-15</span>
       <h3>Your New Post Title</h3>
       <p>Brief description of the post.</p>
       <a href="posts/your-new-post.html" class="read-more">read more →</a>
   </article>
   ```

### Post Template Structure

```html
<!-- Post header with title, date, and tags -->
<!-- Post content with markdown-style formatting -->
<!-- Supported elements: h2, h3, p, ul, ol, code, blockquote, images, tables -->
<!-- Post footer with back button -->
```

## Styling Guide

### Colors
- Primary Background: `#0a0a0f`
- Secondary Background: `#12121a`
- Tertiary Background: `#1a1a24`
- Purple Accent: `#6b2d8a`
- Text Primary: `#e0e0e0`
- Text Secondary: `#9090a0`

### Typography
- Font: Courier New (monospace)
- Headings: 600-700 weight
- Body: 16px base, 1.6-1.8 line height

### Components
- Borders: 1px solid for subtle separation
- Border Radius: 6-8px for modern feel
- Hover Effects: Color shifts, subtle transforms

## Customization

### Change Colors
Edit the CSS variables in `style.css`:
```css
:root {
    --bg-primary: #0a0a0f;
    --purple-accent: #6b2d8a;
    /* ... etc */
}
```

### Modify Layout
All sections are in `index.html`:
- Navigation: Lines 8-18
- Hero: Lines 20-35
- About: Lines 37-48
- Projects: Lines 50-80
- Blog: Lines 82-122
- Social: Lines 154-228

### Add New Sections
Follow the pattern:
```html
<section id="new-section" class="section">
    <div class="container">
        <h2 class="section-title">Title</h2>
        <!-- Your content -->
    </div>
</section>
```

## File Structure

```
├── index.html              # Main landing page
├── style.css              # Global styles
├── post-style.css         # Blog post styles
├── posts/
│   └── post-1.html       # Blog post template
├── favicon.svg           # Site favicon
└── README.md             # This file
```

## Social Media Links

Update these in the "Social" section:

```html
<!-- Hack The Box -->
<a href="https://app.hackthebox.com/profile/156456">

<!-- TryHackMe -->
<a href="https://tryhackme.com/p/syro">

<!-- GitHub -->
<a href="https://github.com/0xsyr0">

<!-- Discord -->
<a href="https://discord.gg/purplestorm">

<!-- X (Twitter) -->
<a href="https://twitter.com/syr0_">

<!-- BlueSky -->
<a href="https://bsky.app/profile/0xsyr0.bsky.social">

<!-- Mastodon -->
<a href="https://infosec.exchange/@syro">
```

## Training and Certifications Sections

The site includes commented-out sections for trainings and certifications. To enable them, simply uncomment the HTML in `index.html` around lines 124-152.

## Contributing

This is a personal site template. Feel free to fork and customize for your own use.

## License

Free to use and modify for personal and commercial projects.

---

Created with caffeine, nightcore and AI
