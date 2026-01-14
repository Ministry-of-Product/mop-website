# Website Redesign - Changes Summary

## Overview
Retailored the Ministry of Product website to match the strategy, tone, and sitemap described in `mop_website_overview.md`. The site now focuses on decision clarity for AI builders with a plainspoken, opinionated, calm tone.

## File Changes

### Configuration
- **`_config.yml`**: Updated site description to "Decision clarity for AI builders. Help making better next-step decisions when you've built something but aren't sure what to do next."

### Core Pages (Rewritten)
- **`index.markdown`** (Home): Completely rewritten with new positioning:
  - Clear value proposition: "Most AI products don't fail because the tech is bad. They fail because the sequence of decisions is wrong."
  - Entry points to Always Be Launching, Advisory, and About
  - Plainspoken, no-hype language
  - Added meta_description for SEO

- **`about.md`** (NEW): Created new About page as perspective statement:
  - Focus on how I think, not résumé
  - Emphasis on judgment, clarity, and restraint
  - Links to advisory for engagement
  - Note: Old `about.markdown` still exists but new `about.md` with permalink takes precedence

- **`always-be-launching.md`** (NEW): ABL hub page:
  - Explains what "Always Be Launching" means
  - Lists recent ABL posts with excerpts and pattern tags
  - Uses Jekyll liquid to filter posts by category

- **`advisory.md`** (NEW): Advisory/guidance page:
  - Fit-focused, no hard sell
  - Clear "who this is for" section
  - Problems it solves
  - Contact modal integration
  - Includes contact form script

- **`manifesto.md`** (NEW): Manifesto page with opinionated statements:
  - Short bullets on launches, progress, decisions, building, getting unstuck
  - Filters audience by alignment with perspective

### Layouts
- **`_layouts/abl_post.html`** (NEW): Template for ABL posts:
  - Structured sections: What They Built, Original Assumption, Where They Got Stuck, Decision That Mattered, What Should Happen Next
  - Pattern tags display
  - Back link to ABL hub
  - Clean, readable structure

### Posts
- **`_posts/2025-01-15-prototype-trap-ai-code-reviewer.md`** (NEW): Example ABL post
  - Pattern: Prototype trap, Overbuilt too early, No clear user
  - Realistic scenario about AI code review tool

- **`_posts/2025-01-20-premature-saas-ai-writing-assistant.md`** (NEW): Example ABL post
  - Pattern: Premature SaaS, Feature vs product, No clear user
  - Realistic scenario about AI writing assistant

- **`_posts/2025-01-25-feature-vs-product-ai-meeting-summarizer.md`** (NEW): Example ABL post
  - Pattern: Feature vs product, No clear user, Overbuilt too early
  - Realistic scenario about AI meeting summarizer

### Includes
- **`_includes/header.html`** (NEW): Navigation header:
  - Fixed position with glass morphism styling
  - Links to Home, Always Be Launching, Advisory, About, Manifesto
  - Responsive design for mobile

- **`_includes/footer.html`**: Updated CTA:
  - Changed from "Contact the Ministry of Product" to "Start a Conversation"
  - Added link to advisory page
  - More aligned with new positioning

- **`_includes/head.html`**: Added meta_description support:
  - Custom meta description tag for SEO
  - Falls back to default description if not specified

### Styles
- **`assets/main.scss`**: Multiple updates:
  - Added `.site-header` and `.site-nav` styles for navigation
  - Added `.abl-post`, `.abl-section`, `.abl-patterns` styles for ABL layout
  - Updated footer link styles
  - Adjusted margin-top for glass-content to account for fixed header
  - Responsive styles for mobile navigation

### Layout Updates
- **`_layouts/default.html`**: 
  - Uncommented header include
  - Navigation now active

## Pages to Review/Archive

### Old Content (Can be archived/removed)
- **`about.markdown`**: Old about page with service-focused content. New `about.md` replaces it via permalink.
- **`_posts/idea_automation/`**: Old idea posts (30+ files). These don't match new positioning and can be archived.
- **`_posts/2023-01-04-welcome-to-the-Ministry-of-Product.markdown`**: Welcome post, can be archived.
- **`catagories/`**: Old category pages (note typo in folder name). These reference old post structure.

### Keep (Working)
- **`404.html`**: Keep as-is
- **`CNAME`**: Keep for domain configuration
- **`favicon.ico`**: Keep
- **`Gemfile` / `Gemfile.lock`**: Keep for Jekyll build
- **`assets/images/OneRoomWorking.png`**: Keep for background
- **Raindrop canvas effect**: Keep (performance optimized)

## New Information Architecture

1. **Home** (`/`) - Trust + framing + entry points
2. **Always Be Launching** (`/always-be-launching/`) - Hub page + individual posts
3. **Advisory** (`/advisory/`) - Conversion page, fit-focused
4. **About** (`/about/`) - Perspective statement
5. **Manifesto** (`/manifesto/`) - Opinionated statements

## SEO Updates

- All pages have `meta_description` in front matter
- Page titles aligned to "decision clarity for AI builders"
- Clean H1 structure (one per page)
- Internal linking between Home ↔ ABL ↔ Advisory ↔ About
- Site description updated in `_config.yml`

## Design Changes

- Navigation header added (fixed, glass morphism)
- ABL post layout with clear section structure
- Pattern tags displayed as badges
- Footer CTA updated to match new tone
- Responsive design maintained
- Typography and spacing optimized for readability

## Content Tone

All copy rewritten to be:
- Plainspoken, not academic
- Opinionated, not preachy
- Calm and confident
- Focused on decisions and sequencing
- No hype language
- No hustle language
- Emphasis on judgment over tools

## Manual Review Checklist

After deployment, review:

- [ ] **Links**: Test all navigation links (Home, ABL, Advisory, About, Manifesto)
- [ ] **ABL Posts**: Verify 3 example posts display correctly with all sections
- [ ] **ABL Hub**: Check that posts are listed correctly with excerpts and pattern tags
- [ ] **Contact Modal**: Test contact button on Advisory page and footer
- [ ] **Mobile**: Test responsive design on mobile devices
- [ ] **Build**: Run `bundle exec jekyll serve` and verify site builds without errors
- [ ] **SEO**: Check page titles and meta descriptions in browser dev tools
- [ ] **Navigation**: Verify fixed header works on scroll
- [ ] **Old Content**: Decide whether to archive/remove old posts in `_posts/idea_automation/`
- [ ] **404 Page**: Test 404 page still works
- [ ] **Background Image**: Verify background image loads correctly
- [ ] **Raindrop Effect**: Test raindrop canvas effect (should work on desktop, disabled on mobile)

## Next Steps

1. Review and test the site locally
2. Decide on archiving old content (idea_automation posts, old about.markdown)
3. Add more ABL posts as real examples come in
4. Consider adding RSS feed for ABL posts
5. Monitor analytics for engagement with new content

