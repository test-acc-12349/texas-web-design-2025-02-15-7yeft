# Texas Web Design Landing Page - Maintenance Guide

This guide will help you maintain and customize the Texas Web Design landing page. It's written for beginners with no prior coding experience.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Fixing and Managing Links](#fixing-and-managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

1. Company Name:
```html
<div class="text-2xl font-bold text-blue-600">
    Texas Web Design  <!-- Change this text -->
</div>
```

2. Navigation Menu Items:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>  <!-- Change menu text here -->
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
Update the main headline and subheading:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6">
    Best Websites In Texas  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Professional web design services that deliver results  <!-- Subheading -->
</p>
```

### Understanding Tailwind Classes
Common classes used in this landing page:
- `text-[size]`: Controls text size (e.g., `text-xl`, `text-2xl`)
- `font-[weight]`: Controls text weight (e.g., `font-bold`, `font-semibold`)
- `mb-[size]`: Adds margin bottom (e.g., `mb-4`, `mb-8`)
- `py-[size]`: Adds padding top and bottom (e.g., `py-24`)
- `bg-[color]`: Sets background color (e.g., `bg-white`, `bg-blue-600`)

## Fixing and Managing Links

### Navigation Menu Links
Current internal links in the navigation:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update these:
1. For internal sections, keep the `#` followed by the section's ID
2. For external pages, use the full URL:
```html
<a href="https://example.com/about">About</a>
```

### Call-to-Action Button
Update the main CTA button link:
```html
<a href="https://twd.com" class="inline-block bg-blue-600 text-white...">
    Get Started Today
</a>
```
Replace `https://twd.com` with your actual website URL.

### Email Contact Link
Update the email address in the CTA section:
```html
<a href="mailto:admin@twd.com" class="inline-block bg-white...">
    Contact Us
</a>
```

## Adding Privacy and Terms Pages

### Footer Links Section
Locate the Legal section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2 text-gray-400">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To link to privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your website directory
2. Update the links:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Links Not Working**
   - Check for typos in URLs
   - Ensure file names match exactly (case-sensitive)
   - Verify files are in the correct directory

2. **Styling Issues**
   - Make sure Tailwind CSS is properly loaded:
   ```html
   <script src="https://cdn.tailwindcss.com"></script>
   ```
   - Check for missing or misspelled classes
   - Ensure responsive classes (md:, lg:) are properly formatted

3. **Content Not Updating**
   - Clear your browser cache
   - Check if you've saved all changes
   - Verify you're editing the correct file

Remember to:
- Always backup files before making changes
- Test all links after updating
- View the page on different devices to ensure responsive design works
- Keep the original HTML structure intact when making changes

Need more help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).