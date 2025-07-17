# XstreamFlex Landing Page Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the XstreamFlex landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Original -->
<a href="/" class="text-2xl font-bold text-gray-900">XstreamFlex</a>

<!-- How to modify -->
<a href="/" class="text-2xl font-bold text-gray-900">Your Company Name</a>
```

#### Hero Section
The hero section contains three key text elements:
1. Main heading
2. Subheading
3. Call-to-action button

```html
<h1 class="text-4xl md:text-6xl font-bold text-white mb-6 tracking-tight">
    Xstream Flex, the Idea Launch Platform
</h1>
<p class="text-xl md:text-2xl text-gray-200 mb-8">
    Take your ideas to full live launch in days not weeks
</p>
```

### Tailwind CSS Classes Explained

Key responsive classes used throughout:
- `md:` - Applies styles on medium screens (768px and up)
- `lg:` - Applies styles on large screens (1024px and up)
- `text-{size}` - Controls font size (xl, 2xl, 3xl, etc.)
- `py-{number}` - Adds padding top and bottom
- `px-{number}` - Adds padding left and right

Example of modifying responsive text:
```html
<!-- Original -->
<h2 class="text-3xl md:text-4xl font-bold text-center mb-16">

<!-- Making text larger -->
<h2 class="text-4xl md:text-5xl font-bold text-center mb-16">
```

## Fixing Broken Links

### Navigation Menu Links
Current navigation links in the header:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
</div>
```

To update internal links:
1. Locate the section ID you want to link to
2. Add a `#` followed by the section ID
3. Example: `<a href="#features">Features</a>`

### Call-to-Action Links
Current CTA links point to:
```html
https://pay.xstreamflex.com/order/starterlaunch/
```

To update:
1. Locate all instances of the CTA link
2. Replace with your payment or signup URL
3. Test each link after updating

## Linking Privacy and Terms Pages

### Footer Policy Links
Current placeholder links:
```html
<ul class="space-y-2 text-gray-400">
    <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    <li><a href="#" class="hover:text-white transition-colors duration-300">Refund Policy</a></li>
</ul>
```

To add proper policy links:
1. Create your policy pages (privacy.html, terms.html, refund.html)
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
<li><a href="refund.html" class="hover:text-white transition-colors duration-300">Refund Policy</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match exactly with href attributes
   - Section IDs are case-sensitive
   - Example: `href="#FAQ"` won't link to `id="faq"`

2. **Responsive Design Issues**
   - Check that you've maintained both mobile and desktop classes
   - Don't remove `md:` or `lg:` prefixes unless intended
   - Test on multiple screen sizes after changes

3. **Image Loading Problems**
   - Verify image URLs are correct and accessible
   - Check image paths relative to your HTML file
   - Ensure images are properly sized and optimized

### Best Practices

1. Always backup before making changes
2. Test all links after updating
3. View changes on multiple devices
4. Maintain consistent spacing and indentation
5. Keep the original class structure when modifying text

Need help? Contact support@xstreamflex.com for assistance.