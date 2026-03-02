# Smart Study Planner - Responsive To-Do List Website

**Student Name:** Aliya Khan

## Live Site URL
https://abkhan79.github.io/CS300-Assignment-2/

## Project Overview
Smart Study Planner is a fully responsive, mobile-first academic to-do list website designed to help students manage their course assignments and deadlines across multiple classes. The site features interactive checkboxes for task tracking, responsive layouts that adapt seamlessly to mobile, tablet, and desktop viewports, and a clean, modern design.

## Viewport Sizes & Responsive Design

### Mobile (Default - under 768px)
- **Layout:** Single-column stacked layout
- **Navigation:** Hamburger menu (collapsible checkbox-driven navigation)
- **Course Cards:** Full-width cards stacked vertically
- **Features:**
  - Optimized touch targets for mobile interaction
  - Readable font sizes (16px+ base font)
  - Proper spacing and padding for mobile screens
  - Images scale to 100% width with proper aspect ratio

### Tablet (768px - 1023px)
- **Layout:** 2-column grid layout
- **Navigation:** Hamburger menu still active
- **Course Cards:** 2×2 grid layout (4 course cards in 2 rows)
- **About Section:** Image and text side-by-side
- **Footer:** 3-column layout for links and social icons
- **Features:**
  - Better use of horizontal space
  - Improved content hierarchy

### Desktop (1024px and above)
- **Layout:** Full-width multi-column layout
- **Navigation:** Horizontal navigation bar (hamburger hidden)
- **Course Cards:** 4-column grid layout (all courses visible in one row)
- **About Section:** 2-column side-by-side with optimized spacing
- **Footer:** Fully expanded 3-column layout
- **Features:**
  - Maximum readability and visual hierarchy
  - Efficient use of screen space
  - Smooth, sticky header navigation

## Screenshots

### Mobile View (375px)
![Mobile screenshot](screenshots/mobile.png)

### Tablet View (768px)
![Tablet screenshot](screenshots/tablet.png)

### Desktop View (1024px)
![Desktop screenshot](screenshots/desktop.png)

## Layout Approach: Mobile-First Design

### Design Philosophy
This project follows a **mobile-first responsive design approach**, where the default CSS styles are optimized for mobile devices, and enhancements are progressively added for larger screens using `min-width` media queries.

### Key Design Decisions

1. **Mobile-First Base Styles**
   - All default CSS targets mobile (smallest screen first)
   - Typography, spacing, and layouts are mobile-optimized
   - Single-column layouts prevent horizontal scrolling
   - Touch-friendly button and checkbox sizes (1.1rem minimum)

2. **Flexbox & CSS Grid**
   - `.feature-grid` uses CSS Grid with responsive `grid-template-columns`
   - Mobile: 1 column (default `display: grid; gap: 1rem`)
   - Tablet (768px): 2 columns
   - Desktop (1024px): 4 columns
   - `.about-layout` and `.footer-layout` also use responsive grid layouts

3. **Responsive Images**
   - All images use `max-width: 100%` and `height: auto`
   - Images scale proportionally across all viewports
   - No fixed image widths that cause overflow

4. **Breakpoints Implementation**
   - **Tablet Breakpoint (768px):** Upgrades grid to 2-column, enables side-by-side footer
   - **Desktop Breakpoint (1024px):** Hamburger hidden, nav becomes horizontal, 4-column grid activated

5. **Content Container**
   - `.container` uses `width: min(100% - 2rem, 1100px)` for responsive padding and max-width
   - Prevents content from stretching excessively on very large screens
   - Maintains readability with proper line lengths

6. **Navigation Behavior**
   - **Mobile:** Checkbox-driven hamburger menu with smooth slide-down animation
   - **Desktop:** Static horizontal navigation bar, hamburger hidden
   - Sticky header remains accessible while scrolling

### No Horizontal Scrolling
- All layouts respect viewport width with proper use of `width: 100%` and `max-width`
- Padding and margins calculated to prevent overflow
- `box-sizing: border-box` applied globally for predictable sizing

## Features

### Header/Navigation
- Logo: "Smart Study Planner"
- 4 Navigation links: Home, Courses, About, Contact
- Mobile hamburger menu with smooth toggle animation
- Sticky positioning for always-accessible navigation

### Hero Section
- Large headline: "My Academic To-Do List"
- Supporting tagline about task management
- Call-to-action button: "View My Tasks"
- Gradient background (dark blue to bright blue)

### Course To-Do Lists (Feature Cards)
1. **CS 300 - Web Development**
   - Individual Project 1: Portfolio Site - Due March 8 at 11:59pm
   - Assignment 2: Responsive Page - Due March 8 at 11:59pm
   - Group 1: Project 1: HTML/CSS/JavaScript Website - Due March 22 at 11:59pm

2. **CS 323 - Cyberlaw**
   - Book Review Presentation - Due before or by March 21 at 3pm

3. **CS 308 - Operating Systems**
   - Design ER diagram for project
   - Write SQL queries for assignment
   - Normalize database schema
   - Present final project proposal

4. **Math 165 - Finite Mathematics For Business And The Social Sciences**
   - Quiz 2 - Due March 3 at 11:59pm

Each card features:
- Course number and title
- Course code in blue color
- Interactive checkboxes for task tracking
- Checked items show strikethrough text

### About Section
- Heading: "Manage Your Academic Success"
- Responsive image from Unsplash (student studying)
- Two paragraphs describing the purpose and benefits of task organization
- Side-by-side layout on tablet/desktop, stacked on mobile

### Footer
- Site branding and tagline
- Quick links to all page sections
- Social media icons (LinkedIn, GitHub)
- Copyright text

## Technical Stack

- **HTML5:** Semantic markup with accessibility features (aria labels)
- **CSS3:** Mobile-first approach with Flexbox and CSS Grid
- **Responsive Design:** Media queries at 768px and 1024px breakpoints
- **No JavaScript:** Pure HTML/CSS functionality (checkbox state managed natively)

## Files Included
- `index.html` - Main HTML file with semantic structure
- `style.css` - Mobile-first responsive styles with media queries
- `README.md` - This documentation file

## Browser Compatibility
Works on all modern browsers supporting:
- CSS Grid
- Flexbox
- CSS `clamp()` function for fluid typography
- CSS custom properties (variables)

## Assignment Completion Checklist
✅ Fully responsive single-page layout
✅ Header with navigation (4+ links) and hamburger menu
✅ Hero section with headline, text, CTA, and background
✅ Feature cards section with 4 course to-do lists
✅ Mobile: Stacked layout and hamburger menu
✅ Tablet: 2-column grid, visible hamburger
✅ Desktop: 4-column grid, horizontal navigation
✅ About section with image and text
✅ Footer with links, social icons, copyright
✅ Mobile-first CSS approach
✅ Min-width media queries (768px, 1024px)
✅ Flexbox and CSS Grid layouts (no floats)
✅ Responsive images with max-width: 100%
✅ No horizontal scrolling at any viewport
✅ Proper use of max-width containers

---

*Last Updated: March 2, 2026*