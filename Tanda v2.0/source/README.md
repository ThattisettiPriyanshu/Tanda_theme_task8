# Overview
This document outlines the standardization work carried out on the Tanda / Fundsweb IT Solutions HTML template project. The goal was to rebrand the template, clean up the original multi-page structure, enforce consistent navigation, update UI aesthetics, and ensure all internal redirections work correctly across every page.

## Original Project Structure
The initial project contained a larger set of files, placeholder text, and generic branding that was not tailored to the Fundsweb identity. It included components that added unnecessary complexity or did not align with a streamlined user experience.

## Standardized Project Structure
After standardization and clean-up, the project was reduced to a clean, minimal set of interconnected pages:

- `index.html` (Home)
- `about-us.html` (Company / About Us)
- `services.html` (Services Overview)
- `services-details.html` (Individual Service Details)
- `blog.html` (Blog)
- `contact.html` (Contact Us)

## What Was Done

### 1. Branding and Content Updates
- Replaced all instances of "Tanda" with "Fundsweb" or "Fundsroom" across meta titles, headers, and footers.
- Updated contact information globally (street address: Nucleus Mall, Pune; email: info@fundsroom.in).
- Removed generic placeholder ("Lorem Ipsum" or "dummy") text and replaced it with meaningful English content suitable for an IT solutions entity.

### 2. Navigation Standardization
All pages were updated to use a consistent main navigation structure:

| Nav Item | Linked Page |
| :--- | :--- |
| **Home** | `index.html` |
| **About Us** | `about-us.html` |
| **Services** | `services.html` |
| **Blog** | `blog.html` |

*Note: The **Contact** link was explicitly removed from the main center navigation to declutter the menu.*

### 3. Header Contact Button
- Replaced the generic "Have any Questions?" section inside the top-right header (`.attr-right`) with a standalone, prominent **"Contact Us"** button that links directly to `contact.html`. 
- This change was replicated across all HTML files for consistency.

### 4. UI & Aesthetic Enhancements
- **Global Background:** Changed the default `body` background color across all pages to a Soft Blue Tint (`#F0F4FF`).
- **Header & Footer:** Updated the main navigation header background to a dark color (`#0d1b2a`) to match the footer, while ensuring navigation links and icons remain visible (white).
- **Top Bar:** Formatted the top bar (containing the address and social links) with a light background (`#F0F4FF`) and dark text (`#1a2238`) for readability.
- **Sliders & Overlays:** Removed slider functionality from the services section in favor of independent, distinct service blocks. Removed unused project overlay icons.

### 5. Redirection Fixes
- All internal `href` links within page content (e.g., service cards, blog categories) were audited and corrected to redirect to the proper standardized pages within the structure. For instance, linking service cards to `services.html` and `services-details.html`.

### 6. Resource Cleanup
- Audited the `assets/img/` folder and removed unused images to keep the project lightweight and clean.

## Notes
- The `assets` folder remains intact and contains all shared CSS (`style.css`, `validnavs.css`), JS, images, and font resources. Custom CSS overrides for the background and header colors were appended to the bottom of `assets/css/style.css`.
- The standardized structure serves as a clean, fully branded base template ready for immediate deployment or further backend integration.
