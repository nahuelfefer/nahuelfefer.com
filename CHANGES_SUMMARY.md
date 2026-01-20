# Website Updates Summary

## Round 2 Changes (Final)

### 1. Email Button Update ✅
- Changed email address from `nahuel@nahuelfefer.com` to `nahuel.s.fefer@gmail.com`
- Removed emoji - button now simply says "Email Me"

### 2. Framework for an Equitable Recovery Image Update ✅
- Updated card image to new version
- New image URL: https://lh3.googleusercontent.com/d/1aLAFAZQy7QKg4PQDkt8tq1xhi65E4S4C

### 3. Enhanced Standalone PDF Pages ✅
All standalone pages now feature:
- **Card image** displayed on the left (300px width)
- **Full card information** including:
  - Date (in gold, uppercase)
  - Title (large navy heading)
  - Description text
  - Download PDF button
- **Improved iframe display:**
  - No black borders (border: none)
  - Taller viewport (90vh instead of 85vh)
  - Better spacing and layout
  - Responsive design that stacks vertically on mobile

Updated pages:
- `cda-impact-report.html`
- `affordable-housing-report.html`
- `roadmap-economic-justice.html`
- `equitable-recovery-framework.html`

### 4. Landing Page Layout Refinement ✅
**Impact Section improvements:**
- **Adjusted column proportions:** Left column (kids photo) is now wider than the two right columns
  - Grid: `2fr 1.5fr 1.5fr` instead of `1fr 1fr 1fr`
  - Kids photo takes up ~40% of width
  - Text/buttons and map each take up ~30%
- **Improved button styling:**
  - Buttons now stack vertically in a cleaner layout
  - Better spacing between elements
  - Max width of 400px for buttons
  - Improved padding and sizing
- **Better visual hierarchy:**
  - Larger "Impact" heading (3.5rem)
  - Slightly smaller subtitle (1.2rem) for better balance
  - Tighter spacing between elements

---

## Original Changes (Round 1)

### 1. Fixed Email Button in About Page ✅
- Updated `about.html` to ensure the "Email Me" button works properly
- Link: `mailto:nahuel@nahuelfefer.com` (later updated to gmail)

### 2. Framework for an Equitable Recovery Card ✅
- Card already existed in `work.html` with correct information:
  - Date: April 2021
  - Title: Framework for an Equitable Recovery
  - Description: Jones Transition Team plans for deployment of $500M in ARPA funds. Most, though not all, of these proposals were ultimately implemented.
  - Image: https://lh3.googleusercontent.com/d/1jF0kHGY_gpLbt-0l4FvwtQBS2YW4S4-5
- **Moved card from Legislation section to Reports & Memos section**
- **Placed in correct chronological position** (between April 2022 Roadmap and November 2019 Equitable Unification)
- Links to standalone page: `equitable-recovery-framework.html`
- PDF embedded: https://drive.google.com/file/d/1H5X9tyXt-MELR0SpTO65bd9MRZqnqUcl

### 3. Created Standalone Pages for Google Drive PDFs ✅
All Google Drive PDF links now have dedicated pages with embedded PDFs under the website header and footer.

**New standalone pages created:**
1. `affordable-housing-report.html` - City of St. Louis Affordable Housing Report (November 2023)
2. `roadmap-economic-justice.html` - Roadmap to Economic Justice (April 2022)

**Updated links in work.html:**
- Changed direct Google Drive links to point to standalone pages for:
  - Affordable Housing Report
  - Roadmap to Economic Justice
  - Equitable Unification Report
  - NYC Property Tax Reform

**Existing standalone pages verified:**
- `cda-impact-report.html`
- `charter-reform.html`
- `equitable-unification.html`
- `nyc-property-tax-reform.html`
- `equitable-recovery-framework.html`
- `investments-map.html` (links to the Neighborhood Transformation Investments Map PDF)
- And many others throughout the site

All standalone pages follow the same template:
- Header with site navigation
- PDF title
- Download PDF button
- Embedded PDF viewer (using Google Drive preview)
- Footer with sitemap and contact info

### 4. Updated Landing Page (index.html) ✅
**Impact Section redesign:**
- Changed from 2-column to 3-column layout
- **Left column:** Kids at playground photo (existing)
- **Center column:** 
  - "Impact" heading
  - Updated subtitle: "Investing in Neighborhoods & Housing" (changed from "Investing $250M+ into Neighborhoods & Housing")
  - Two buttons stacked vertically (both now link to standalone pages):
    - Read Community Development Impact Report → `cda-impact-report.html`
    - Explore Interactive Map of Investments → `investments-map.html`
- **Right column:** New clickable map image
  - Image: https://lh3.googleusercontent.com/d/1kUAZDMMMa4wTc8UAVHftrzxeBYDsvKLd
  - Links to: `investments-map.html` 
  - Which embeds PDF: https://drive.google.com/file/d/1JTOvYnWQlHZ84k2F-PXw_ZCcBrnsg6hd

**CSS Updates:**
- Grid changed to 3 columns with equal spacing
- Images are same height with proper scaling
- Added hover effect on map image (slight zoom)
- Centered all text and buttons between the two images

## Technical Notes

All standalone PDF pages use the same structure:
```html
- Header (consistent with rest of site)
- PDF container with:
  - Title
  - Download button (links to Google Drive)
  - Embedded iframe (using /preview URL for better embedding)
- Footer (consistent with rest of site)
```

Google Drive embed format used:
- Download link: `https://drive.google.com/file/d/[FILE_ID]/view?usp=sharing`
- Embed iframe: `https://drive.google.com/file/d/[FILE_ID]/preview`

## Files Modified
1. `about.html` - Fixed email button
2. `index.html` - Updated Impact section layout and subtitle
3. `work.html` - Moved Framework card to correct position, updated Google Drive links to standalone pages
4. `affordable-housing-report.html` - NEW FILE
5. `roadmap-economic-justice.html` - NEW FILE

## Files Verified (Already Correct)
- `equitable-recovery-framework.html` - Framework for an Equitable Recovery standalone page
- `investments-map.html` - Neighborhood Transformation Investments Map standalone page
- `media.html` - All links already point to standalone pages
- Various other standalone pages for essays, reports, and legislation

All changes maintain the existing design aesthetic with navy (#1a3a52) and gold (#d4a855) color scheme.
