# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. It's designed for beginners and provides detailed instructions for common updates and modifications.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. **Logo Text**
```html
<div class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
    Logo <!-- Replace "Logo" with your company name -->
</div>
```

2. **Navigation Menu Items**
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <!-- Update text between <a> tags for each menu item -->
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
    Lorem ipsum dolor <!-- Replace with your headline -->
</h1>
<p class="text-xl text-gray-600 mb-12 leading-relaxed">
    Lorem ipsum dolor sit amet <!-- Replace with your subheading -->
</p>
```

### Tailwind CSS Class Guide
- Text sizes: `text-sm`, `text-base`, `text-lg`, `text-xl`, etc.
- Colors: `text-gray-600`, `bg-purple-600`, etc.
- Spacing: `px-6` (padding left/right), `py-4` (padding top/bottom), `mb-8` (margin bottom)
- Responsive classes: `md:text-5xl` (applies at medium screens and up)

## Managing Links

### Navigation Menu Links
Current placeholder links need updating:

```html
<!-- In the header navigation -->
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a> <!-- Change "#" to actual section ID or page URL -->
    <a href="#benefits">Benefits</a>
    <a href="#contact">Contact</a>
</div>
```

### Call-to-Action (CTA) Buttons
Update these important links:

```html
<!-- Hero section CTA -->
<a href="/signup" class="inline-block bg-gradient-to-r...">
    Get Started Now <!-- Add your signup or landing page URL -->
</a>

<!-- Bottom CTA section -->
<a href="/start" class="inline-block bg-white...">
    Start Now <!-- Add your getting started page URL -->
</a>
```

### How to Update Links
1. Find the `<a>` tag you want to update
2. Modify the `href` attribute with your URL:
   - Internal page: `href="about.html"`
   - Section link: `href="#features"`
   - External link: `href="https://example.com"`

## Adding Privacy and Terms Pages

### Footer Link Updates
Locate the legal section in the footer:

```html
<div>
    <h4 class="text-sm font-semibold uppercase tracking-wider text-gray-900 mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="privacy.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Privacy</a></li>
        <li><a href="terms.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Terms</a></li>
    </ul>
</div>
```

### Steps to Add Policy Pages
1. Create new files:
   - Create `privacy.html` in your root directory
   - Create `terms.html` in your root directory
2. Update the href attributes in the footer links
3. Maintain consistent styling by copying the header and footer from index.html

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check for typos in URLs
   - Ensure files exist in the correct directory
   - Verify file names match exactly (case-sensitive)

2. **Responsive Design Issues**
   - Check responsive classes (md:, lg:, etc.)
   - Test on different screen sizes
   - Don't remove `viewport` meta tag in header

3. **Styling Problems**
   - Verify Tailwind CSS CDN link is working
   - Check for missing or mistyped classes
   - Ensure class names are spelled correctly

### Getting Help
- Check [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Validate HTML at [W3C Validator](https://validator.w3.org/)
- Test responsive design using browser dev tools (F12)

## Best Practices
- Always backup files before making changes
- Test all links after updating
- Check your page on multiple devices
- Keep consistent styling across all pages
- Maintain the same structure in new pages
- Comment your code for future reference

Remember to replace all placeholder text (Lorem ipsum) with your actual content before publishing the site.