# About Page Refactoring - File Manifest

This file provides an overview of the components and changes made to refactor the About page based on the legacy website design.

## New Components Created

1. **TeamMember.astro**
   - A reusable component for displaying team member information
   - Includes support for social media links (LinkedIn, GitHub, Twitter)
   - Uses a clean card-based design with hover effects

2. **MissionVision.astro**
   - A flexible component for displaying mission, vision, or values sections
   - Supports image + text layout with optional reversed positioning
   - Handles multiple paragraphs and HTML content

3. **Section.astro**
   - A versatile section component with consistent styling
   - Supports various background styles (default, light, dark, primary)
   - Includes title, subtitle, and content areas

## Files Modified

1. **about.astro**
   - Complete rewrite to use the new component structure
   - Added sections for:
     - Who We Are
     - Mission & Values
     - Team
     - Our Approach
   - Improved responsive design

2. **global.scss**
   - Added CSS variables for consistent theming
   - Expanded color palette
   - Added structural and typography variables

## Images Used

1. **team-placeholder.jpg** (newly added)
   - Placeholder for team member photos

2. **atlanta-hero-image.jpeg** (existing)
   - Used for the mission section

3. **noclocks-logo.png** (existing)
   - Used for the values section

## Structure

The refactored About page follows a modular, component-based architecture that makes it:
- Easier to maintain
- More consistent with design patterns
- Responsive across different device sizes
- Aligned with the original legacy site's content and structure

## Design Considerations

1. Used a clean, modern aesthetic consistent with the No Clocks brand
2. Maintained the dark theme with appropriate contrast
3. Added interactive elements (hover states, transitions)
4. Ensured accessibility with proper headings and semantic structure
