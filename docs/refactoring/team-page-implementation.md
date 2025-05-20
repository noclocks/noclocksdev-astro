# Team Page Implementation

This document outlines the implementation of the dedicated team page and how it integrates with the rest of the No Clocks website.

## Overview

The team information is now represented in multiple places:

1. **About Page**: Contains a condensed team section with basic info and a link to the full team page
2. **Team Page**: A dedicated page showing detailed team member profiles
3. **Markdown Files**: Source of truth for team member information in `docs/website/team/`

## File Structure

- `src/pages/team.astro` - Main team page template
- `src/components/TeamMember.astro` - Reusable component for team member cards
- `docs/website/team/*.md` - Markdown files containing team member information

## Content Management

Team member information is maintained in markdown files under `docs/website/team/`. These files include:

- Name, role, and contact information
- Detailed biography
- Social media links
- Image path references

Example structure:
```markdown
# Jimmy Briggs

## Information
- **Name**: Jimmy Briggs
- **Role**: CTO | Co-Founder | Full Stack Developer
- **Email**: jimmy.briggs@noclocks.dev

## Image
![Jimmy Briggs](../assets/images/team/jimmy-briggs.png)

## Biography
...

## Links
- **GitHub**: [jimbrig](https://github.com/jimbrig)
- **LinkedIn**: [Jimmy Briggs](https://www.linkedin.com/in/jimbrig)
```

## Navigation

The site navigation has been updated to include a dedicated "Team" link, making the team page accessible from anywhere on the site.

## Images

Team member images are stored in `public/images/team/` with the naming convention `firstname-lastname.png`.

## Implementation Notes

1. **About Page Team Section**:
   - Provides a brief introduction to the team
   - Shows simplified team member cards for key members
   - Includes a CTA button to the full team page

2. **Team Page**:
   - Showcases all team members with detailed information
   - Includes fuller biographies and contact information
   - Alternates layout direction for visual interest

3. **TeamMember Component**:
   - Reusable component used on both pages
   - Supports LinkedIn, GitHub, and Twitter links
   - Has default fallback image if no image is provided

## Future Enhancements

1. **Content Management**: Consider implementing a more streamlined content management approach that could automatically generate team pages from markdown files using Astro's content collections feature

2. **Team Member Detail Pages**: Could add individual pages for each team member with more detailed information, portfolios, and project showcases

3. **Dynamic Image Loading**: Implement responsive image loading strategies for optimized performance

## Maintenance Guidelines

When adding or updating team members:

1. Create or modify the markdown file in `docs/website/team/`
2. Add the team member's image to `public/images/team/`
3. Update the `teamMembers` array in `src/pages/team.astro`
4. Consider updating the About page if the person is a key team member
