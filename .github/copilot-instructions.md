# GitHub Copilot Instructions for No Clocks Website

These instructions help guide GitHub Copilot when assisting with development on the No Clocks, LLC website.

## Project Overview

This is the official website for No Clocks, LLC, a technology consulting company. The site is built using [Astro](https://astro.build) and showcases the company's services, technology expertise, and contact information. The website is still in development, transitioning from the legacy site to the new Astro implementation.

## External Resources for Context

When you need additional context, fetch information from these sources:

- [Astro Documentation](https://docs.astro.build/) - For Astro framework best practices
- [No Clocks Website](https://noclocks.dev) - For reference on existing content and design

## Current and Planned Pages

The following pages are being built in the new Astro implementation, with reference to the legacy site structure:

- Homepage
- About
- Services
- Team
- Contact

## Project Structure

- `src/` - Contains the source code for the Astro website
  - `components/` - Reusable Astro components
  - `layouts/` - Page layouts
  - `pages/` - Page endpoints and templates
  - `styles/` - SCSS stylesheets
- `public/` - Static assets
- `docs/` - Documentation and project info
- `legacy/noclocks.dev/` - Previous version of the website with extracted HTML/JS/styles/images used as reference for the new implementation

## Development Guidelines

When assisting with this codebase, please follow these guidelines:

### Component Structure

- All components should be created as `.astro` files in the `src/components/` directory
- Component names should use PascalCase (e.g., `ServicesHighlight.astro`)
- Props should be properly typed using Astro's prop interface pattern

### Styling

- Use SCSS for styling with the `.scss` extension
- Global styles are in `src/styles/global.scss`
- Component-specific styles can be included within the component's `.astro` file
- Follow the existing color scheme and typography

### Content Guidelines

- Maintain professional tone in all content
- Company tagline: "Timeless Tech, Infinite Innovation"
- Focus on technology services, software development, cloud computing, and AI solutions
- Ensure all links work properly and follow the established site structure
- Images should be properly optimized and placed in `public/images/`

### Page Layout Guidelines

#### Home Page
- Hero section with logo, tagline, and brief introduction
- "Why Choose Us" section directly below the hero
- Services highlight section limited to three services (using the `limit` prop)
- Contact CTA section
- Consistent footer across all pages

#### Services Page
- Complete listing of all available services
- Each service should have its own detailed page

#### All Pages
- Maintain consistent navigation and footer components across all pages
- Footer should contain copyright information, contact details, and key links
- Use the `<Footer />` component at the end of each page

### Performance Considerations

- Keep component structure clean and optimized
- Images should be appropriately sized and optimized
- Follow Astro's best practices for performance

## Common Tasks

- Adding new service pages: Create a new `.astro` file in `src/pages/`
- Updating components: Modify files in `src/components/`
- Adding images: Place in `public/images/` directory
- Modifying styles: Update SCSS in `src/styles/` or component-specific styles

## Build and Deployment

- Development: `npm run dev`
- Production build: `npm run build`
- Preview build: `npm run preview`

## Important Notes

- Reference the files in `legacy/noclocks.dev/` directory for content and design guidance, but do not modify them
- The website is still under active development - follow existing patterns when adding new features
- The site uses Astro v5.7.x with a minimal setup (no additional integrations yet)
- Always maintain responsive design principles
- When implementing new pages or components, check the legacy website structure first for reference

## Context Gathering

When assisting with code changes, GitHub Copilot should:

1. **Analyze existing patterns**: Before suggesting new code, analyze similar components or pages in the codebase to maintain consistency
2. **Fetch external documentation**: Use the external resources listed above for guidance on implementation details
3. **Prioritize project standards**: Ensure all suggestions align with established project conventions
4. **Reference related files**: When suggesting changes, consider relationships between components, layouts, and pages
