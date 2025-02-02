# Easy Grip Utensils Landing Page - Maintenance Guide

This guide will help you maintain and customize the Easy Grip Utensils landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Policy Pages](#adding-policy-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu:

```html
<div class="text-xl font-bold text-gray-800">MazalCrafts</div>
```
To change the company name:
1. Locate this div in the header section
2. Replace "MazalCrafts" with your desired name
3. Adjust text size using Tailwind classes if needed:
   - `text-xl` (current) - medium large
   - `text-2xl` - larger
   - `text-lg` - slightly smaller

### Hero Section
To update the main headline and subtext:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-8">
    🍽 Easy Grip Utensils for Arthritis & Seniors
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Regain Your Mealtime Independence with Easy Grip Utensils
</p>
```

Key classes explained:
- `text-4xl/5xl/6xl`: Responsive text sizing
- `md:` and `lg:`: Screen size breakpoints
- `mb-8/12`: Margin bottom spacing

### Features Section
Each feature card follows this structure:

```html
<div class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition duration-300">
    <div class="text-blue-600 text-4xl mb-4">
        <i class="fas fa-hand-holding"></i>
    </div>
    <h3 class="text-xl font-bold mb-4">Ergonomic Non-Slip Handles</h3>
    <p class="text-gray-600">Your description here</p>
</div>
```

To modify features:
1. Locate the features section (`id="features"`)
2. Update icon by changing the `fas fa-*` class
3. Modify heading text in the `<h3>` tag
4. Update description in the `<p>` tag

## Managing Links

### Navigation Menu Links
Current navigation links are:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-blue-600 transition duration-300">Features</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600 transition duration-300">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600 transition duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition duration-300">Contact</a>
</div>
```

To update links:
1. Modify `href` attributes to point to new sections
2. Ensure section IDs match in the HTML
3. Keep the `#` prefix for internal page links

### Shop Now Buttons
The page contains two "Shop Now" buttons. Update the affiliate link in both locations:

```html
<a href="https://shareasale.com/r.cfm?b=2278&u=1520322&m=942&urllink=www%2Earthritissupplies%2Ecom%2Feating%2Dutensils%2Ehtml%3Fsrsltid%3DAfmBOoqgEpN3X94ErTandD58D1WsW2PV4r54O3S1d3jbzErUOx2EBWeH&afftrack=" class="inline-block bg-blue-600 text-white px-8 py-4 rounded-lg text-lg font-semibold hover:bg-blue-700 transform hover:scale-105 transition duration-300">Shop Now</a>
```

## Adding Policy Pages

### Footer Policy Links
Current placeholder links in the footer:

```html
<ul class="space-y-2">
    <li><a href="#" class="hover:text-white transition duration-300">Privacy Policy</a></li>
    <li><a href="#" class="hover:text-white transition duration-300">Terms of Service</a></li>
    <li><a href="#" class="hover:text-white transition duration-300">Returns Policy</a></li>
</ul>
```

To link policy pages:
1. Create your policy pages (e.g., `privacy.html`, `terms.html`)
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Internal Links**
   - Ensure section IDs match navigation href attributes
   - Section IDs should not include spaces
   - Check for proper # prefix in href

2. **Responsive Design Issues**
   - Don't remove `md:` or `lg:` prefixes from classes
   - Maintain the responsive grid structure in features/benefits sections
   - Keep the `container` class on main wrapper divs

3. **Icon Problems**
   - Verify Font Awesome CDN is loaded
   - Check icon class names against [Font Awesome documentation](https://fontawesome.com/icons)
   - Ensure proper prefix (`fas`, `fab`, etc.)

For additional help or questions, refer to:
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Font Awesome Icons](https://fontawesome.com/icons)
- Your web development team or support resources