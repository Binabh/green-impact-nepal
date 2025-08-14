# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### CSS Build and Watch
```bash
npx tailwindcss -i ./docs/input.css -o ./docs/output.css --watch
```
This command processes Tailwind CSS and should be run when making style changes.

### Install Dependencies
```bash
npm install
```
Installs Tailwind CSS and other development dependencies.

## Project Architecture

This is a modern multi-page website for Green Impact Nepal (GIN), an environmental NGO focused on forest conservation and climate change awareness. The project has been redesigned with a modern approach:

### File Structure
- **Website root**: `docs/` directory contains the deployable website
- **Main page**: `docs/index.html` - Modern homepage with card-based layout
- **Article pages**: `docs/articles/` - Individual pages for each project/program
- **Styling**: Uses Tailwind CSS with custom animations and modern design system
- **Assets**: Images and media files in `docs/assets/`
- **Configuration**: `tailwind.config.js` with custom animations and modern styling

### Modern Design Features
- **Card-based layout**: Clean, modern cards for project showcases
- **Custom animations**: Fade-in, slide-up, float, and gentle bounce animations
- **Responsive design**: Mobile-first approach with breakpoint-specific layouts
- **Subtle interactions**: Hover effects, transitions, and micro-animations
- **Modern typography**: Improved spacing, hierarchy, and readability
- **Color-coded sections**: Each project type has its own color scheme

### Content Architecture
- **Home**: Modern hero section with floating animations and improved CTA
- **About**: Card-based vision/mission layout with icons
- **Works**: Separated into "Ongoing" and "Completed" projects with modern cards
- **Individual Articles**: Dedicated pages for each project with comprehensive content
- **Contact**: Modern contact cards with improved visual hierarchy

### Navigation
- Modern sticky navigation with backdrop blur
- Smooth hover transitions and color changes
- Breadcrumb navigation in article pages
- Mobile-responsive hamburger menu (if needed)

### Article System
Each article page (`docs/articles/*.html`) follows a consistent structure:
- **Header section**: Gradient background with project title and category
- **Image gallery**: Showcasing related project photos
- **Content sections**: Well-structured content with modern typography
- **Status badges**: Visual indicators for project status
- **Navigation**: Back to main works section

### Animation System
Custom Tailwind animations defined in `tailwind.config.js`:
- `fade-in`: Smooth entrance animations
- `slide-up`: Content reveal animations
- `bounce-gentle`: Subtle attention-grabbing animations
- `float`: Gentle floating effect for hero images

### Deployment
The website is configured for GitHub Pages deployment with `docs/CNAME` file present.

## Development Notes

- **Modern approach**: No modals - each project has its own dedicated page
- **Performance optimized**: Uses CSS animations instead of JavaScript where possible
- **SEO friendly**: Each article has proper meta tags and structured content
- **Maintainable**: Clean separation between main page and article content
- **Accessible**: Proper semantic HTML and ARIA considerations
- **Build system**: Requires Tailwind CSS compilation for styling changes