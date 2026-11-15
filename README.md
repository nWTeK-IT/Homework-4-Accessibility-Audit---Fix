# The Codenote
## Project Milestone 3 — Accessible & Designed

**Current status:** In progress — visual design documentation added; contact form and final verification pending.

**Developer:** Jason Marsden  
**Project:** The Codenote — Personal Portfolio Website  
**Course:** Web Development  
**Last updated:** November 15, 2026  
**Technologies:** HTML5, CSS3, Git, GitHub, GitHub Pages

---

## Project Overview

The Codenote is a personal portfolio website created to
showcase my journey as an Information Technology student
at Campus.edu.

The website features a Death Note-inspired design,
combining custom typography, dark colors, animations,
and responsive layouts.

Milestone 2 established the site's styling and responsive layouts across desktop, tablet, and mobile devices. Homework 4 introduced accessibility fixes. Milestone 3 builds on that work with intentional Gestalt design, contrast verification, and an accessible contact form.

---

## Project Objectives

The objectives of the earlier styling and responsive milestone were to:

- Implement an external CSS stylesheet.
- Establish a consistent visual design.
- Apply custom fonts and typography.
- Improve spacing and page organization.
- Use CSS Grid and Flexbox for layout management.
- Implement responsive design using media queries.
- Ensure compatibility with mobile, tablet, and desktop screens.
- Test the website using browser Developer Tools.
- Publish and maintain the website through GitHub Pages.

---

## Website Structure

The website consists of three primary HTML pages:

### Home — index.html

The homepage introduces The Codenote and includes:

- Website logo and branding.
- Navigation menu.
- Welcome message.
- Animated Kira GIF.
- Introduction to my IT education and career goals.
- Footer containing copyright information and a LinkedIn link.

### About — about.html

The About page provides information about my background,
education, and interests in Information Technology.

### Projects — projects.html

The Projects page is dedicated to showcasing my
development projects and technical accomplishments.

---

## Milestone 3 Development Log — November 15, 2026

### Accessibility work carried forward from Homework 4

- **Heading order:** Corrected heading hierarchy to improve document structure for assistive technologies.
- **Image description:** Replaced the ambiguous reference to Kira with a description identifying Light Yagami from Death Note.
- **Redundant navigation:** Removed unnecessary duplicate links, including the separate Home link when the logo already navigates home, and current-page links on the About and Projects pages.

These changes were made during Homework 4; a new WAVE scan of all three pages is still needed after the Milestone 3 form is added.

### Visual Design — Gestalt Principles

**1. Proximity:** I used proximity to group related elements, including the logo, site title, and navigation in the header. Spacing and borders separate the welcome section from other content, making the page easier to scan.

**2. Similarity:** I used similarity through consistent typography, navigation styling, gray borders, and repeated colors across the Home, About, and Projects pages. These recurring design elements help visitors recognize the same website as they navigate.

### Color Palette and Contrast

The Death Note-inspired palette uses black backgrounds (`#000000`), white text (`#ffffff`), and gray borders (`#555555`). The navigation hover uses dark red (`#9b1c31`), and the footer hover uses muted green (`#6f9b82`).

**Contrast verification pending:** White on black meets WCAG AA, but the existing dark-red navigation hover text against black does not meet the 4.5:1 minimum for normal text. The red can remain as a decorative accent, but interactive text needs a passing foreground/background combination before final submission. Verify all text/background states with the WebAIM Contrast Checker.

### Accessible Contact Form — Planned

Add a contact form to `about.html` with explicitly associated `label` elements, appropriate `fieldset` and `legend` grouping, keyboard accessibility, and programmatically associated validation errors. Because GitHub Pages hosts static sites, form submission or message delivery requires a separate service or backend if that behavior is desired.

### Final Submission — Pending

- [ ] Complete and test the accessible contact form.
- [ ] Verify all text/background combinations against WCAG AA.
- [ ] Run WAVE on Home, About, and Projects after the changes and resolve every error.
- [ ] Update this README with actual final fixes and testing results.
- [ ] Commit and push the finished site and submit the final GitHub repository URL.

---

## Milestone 2 Development Log — November 1, 2026

### 1. Responsive Header Improvements

Modified the website's header styling to improve
its appearance on smaller screens.

Changes included:

- Adjusting header padding.
- Improving CSS Grid positioning.
- Correcting mobile layout alignment.
- Preventing content from extending beyond the screen.
- Improving the placement of the website logo.

### 2. Mobile Layout Adjustments

Implemented and refined a mobile media query targeting
screens 600 pixels wide or smaller.

The mobile layout adjusts the header, navigation,
logo positioning, and other page elements to fit
smaller displays.

Example:

    @media (max-width: 600px) {
        /* Mobile-specific styling */
    }

### 3. Responsive GIF Improvements

Identified an issue where the animated Kira GIF
was wider than the mobile screen.

This caused horizontal scrolling and affected
the appearance of other page elements.

Corrected the issue using responsive CSS:

    .Kira-gif {
        width: 100%;
        max-width: 100%;
        height: auto;
    }

These properties allow the GIF to scale according
to its available space while maintaining its
original proportions.

### 4. Mobile Logo Alignment

Adjusted the Codenote logo to appear centered
above the website title on mobile screens.

Used the following CSS property:

    justify-self: center;

This improved the visual alignment of the
mobile header.

### 5. Tablet Media Query

Added a second media query targeting screen
widths between 601 and 900 pixels.

    @media (min-width: 601px) and (max-width: 900px) {
        .site-header {
            padding: 16px 24px;
        }
    }

This provides tablet-specific header spacing
without requiring a complete redesign.

### 6. Browser Cache Troubleshooting

Encountered an issue where the published website
displayed an outdated logo position on a mobile device.

The local Live Server preview displayed the
correct positioning.

After testing the website using a mobile browser's
incognito mode, the correct layout appeared.

This helped identify browser caching as the
cause of the inconsistent appearance.

### 7. Live Server Installation

Installed the Live Server extension in
Visual Studio Code.

Live Server provides a local development
environment that automatically refreshes
the webpage when changes are saved.

This improved the development workflow by
reducing the need to repeatedly commit changes
and wait for GitHub Pages deployment.

### 8. Responsive Design Testing

Tested the website using Chrome Developer Tools
and responsive device emulation.

The following screen widths were tested:

| Device | Screen Width | Result |
|--------|--------------|--------|
| Mobile | 320px | Passed |
| Tablet | 768px | Passed |
| Desktop | 1200px | Passed |

All three screen widths displayed correctly
during testing.

The tablet layout was tested again after
adding the second media query.

No additional layout problems were reported.

---

## Responsive Design Implementation

The website uses three responsive screen ranges.

### Desktop — 901px and Above

The desktop layout uses the default CSS styling.

No separate desktop media query is required
because the original CSS rules apply automatically.

### Tablet — 601px to 900px

A tablet-specific media query adjusts header
padding while retaining the existing layout.

### Mobile — 600px and Below

The mobile media query adjusts the website
layout for smaller screens.

These changes include responsive images,
header adjustments, and logo alignment.

---

## Tools and Technologies

### HTML5

Used to structure the website's content,
navigation, sections, and footer.

### CSS3

Used for visual styling, typography,
spacing, responsive images, and layout.

### CSS Grid and Flexbox

Used to organize page elements and manage
responsive layouts.

### Media Queries

Used to apply different styling rules
depending on browser width.

### Visual Studio Code

Used as the primary development environment.

### Live Server

Used to preview changes locally and
automatically refresh the website.

### Chrome Developer Tools

Used to inspect elements, troubleshoot CSS,
and test responsive screen sizes.

### Git and GitHub

Used for version control and maintaining
the project's source code.

### GitHub Pages

Used to publish the website online.

---

## Challenges and Solutions

### Challenge: Mobile Content Overflow

**Problem:**
Some website elements extended beyond the
mobile screen, creating horizontal scrolling.

**Solution:**
Adjusted responsive CSS properties and
corrected the oversized animated GIF.

### Challenge: Logo Alignment

**Problem:**
The website logo appeared incorrectly positioned
on mobile devices.

**Solution:**
Adjusted the logo's CSS alignment and verified
its appearance using responsive testing.

### Challenge: Inconsistent Published Appearance

**Problem:**
The local website displayed correctly while
the mobile browser showed outdated styling.

**Solution:**
Tested the published website in incognito mode
and identified browser caching as the issue.

### Challenge: Slow Development Workflow

**Problem:**
Repeatedly waiting for GitHub Pages deployment
made testing small CSS changes time-consuming.

**Solution:**
Installed Live Server to preview changes
immediately after saving files.

---

## Testing Results

Responsive testing confirmed that the website
displayed correctly at the three required
screen widths.

- Mobile: 320 pixels
- Tablet: 768 pixels
- Desktop: 1200 pixels

The website uses two CSS media queries
alongside its default desktop styling.

---

## Conclusion

Project Milestone 2 focused on transforming
The Codenote into a styled and responsive
personal portfolio website.

Throughout development, I improved my
understanding of CSS, media queries,
responsive images, browser Developer Tools,
and GitHub Pages deployment.

I also learned how browser caching can
affect the appearance of published websites
and how Live Server can improve the
development and testing process.

The website has been tested successfully
at mobile, tablet, and desktop screen widths.

These improvements establish a foundation
for future development of The Codenote.

---

**Developed by Jason Marsden**  
**Last updated November 15, 2026**