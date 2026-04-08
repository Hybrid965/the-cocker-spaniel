# The Cocker Spaniel

## Purpose
**The Cocker Spaniel** is an informational website created for prospective dog owners who are researching breeds but are overwhelmed by lengthy, technical resources. The target audience is families and first-time dog owners who want a clear, friendly, and visually engaging introduction to the breed before committing to ownership. The goal is that a visitor can arrive and, within minutes, have a confident understanding of whether a Cocker Spaniel suits their lifestyle.

## User Stories
### As a prospective owner:
- As a prospective dog owner, I want to quickly understand the Cocker Spaniel's personality so that I can decide if the breed suits my lifestyle.
- As a prospective owner, I want to see key facts at a glance so that I don't have to read lengthy text to get basic information.
- As a prospective owner, I want to understand the grooming commitment so that I can decide if I have the time and budget for the breed.
### As a parent/family:
- As a parent, I want to know if Cocker Spaniels are good with children so that I can feel confident bringing one into my home.
- As a family owner, I want to understand the breed's energy levels so that I can plan appropriate exercise and activities.
### As a first-time dog owner:
- As a first-time dog owner, I want clear and friendly information so that I don't feel overwhelmed by technical or medical jargon.
- As a first-time owner, I want to understand how trainable the breed is so that I know what to expect when bringing a puppy home.
## UX Design
### Strategy Plane
- **Target Audience**: Prospective Owners, Families and first-time dog owners.
- **User Needs**: Accessible information on temperament, exercise needs, and grooming.
- **Rationale**: The project provides a clear, well-defined purpose addressing the needs of specific audiences by simplifying information into a user-centric digital experience.
### Scope Plane
- **Project Requirements**: A fully responsive three-page application featuring intuitive navigation and section-specific anchor links.
- **Content Requirements**: Breed facts & statistics, structured feeding tables, grooming summary cards, and a chronological history timeline.
### Structure Plane
- **Information Hierarchy**: Information is categorized by priority. Headers are used to convey structure, with the most vital "Quick Facts" (Size, Lifespan, Energy) placed at the top of the Home page for immediate access.
- **Interaction Feedback**: The site provides clear confirmation of user actions; for example, the active page link is highlighted in the navbar.
- **User Control**: The site avoids aggressive automatic pop-ups and auto-play; all interactions, including navigation and media viewing, are initiated and controlled by the user.

### Skeleton Plane
- **Wireframes**: Initial layouts were designed for all pages to plan the placement of headers, images, and navigation menus.
 - 📄 [Home](docs/wireframes/home.png)
 - 📄 [Care](docs/wireframes/care.png)
 - 📄 [History](docs/wireframes/history.png)

- **Old Wireframes**:
- 📄 [Care Desktop](docs/wireframes/care-old.png)
- 📄 [Care Mobile](docs/wireframes/care-phone-old.png)
- **Layout Changes**: The Care page wireframe originally placed content in a left-aligned layout with the grooming image sitting alongside the text. During development this was changed to a centralised layout, with content sections stacked and centred on the page. This decision was made to improve readability and create a cleaner, more focused user experience.
- **Navigation Design**: A fixed navigation bar ensures that primary resources are easy to find and accessible across all screen sizes.
### Surface Plane
- **Colour Palette**: The site uses a consistent colour palette across all pages. Deep navy (`#122c47`) is used for the navigation bar and primary headings, providing strong contrast against lighter backgrounds. Saddle brown (`#8b4513`) is used for subheadings. Body text uses a muted warm brown (`#7a6a58`) to maintain contrast against white and light backgrounds. The History page intentionally uses an older style coloured background (`#f2e8d5`) to make the content feel more historical.
- **Font**: Playfair Display (headings) and Lato (body) are paired to maintain a balance between a "historical" aesthetic and modern readability.
- **Accessibility & Imagery** : All images include descriptive alt text. Semantic HTML elements are used throughout to provide a clear document structure for screen readers. ARIA labels have been used to further aid screen readers.
## Features

### Across All Pages

- **Responsive Navigation**: A fixed navigation bar sits at the top of every page with links to Home, Care and History. The active page link is highlighted so users always know where they are. The navbar is fully responsive and stacks cleanly on smaller screens.
- **Hero Anchor Links**: Each page opens with a full-width hero featuring a bold headline and tagline. The Care and History heroes include anchor links - Grooming, Nutrition and Exercise on Care; Origins, Timeline and Breeds on History - letting users jump straight to the section they need.
- **Fully Responsive Design**: All three pages adapt across desktop, tablet and mobile screen sizes using CSS media queries. Multi-column layouts stack vertically on smaller screens and images scale proportionally throughout.
- **Footer**: A consistent footer across all three pages includes navigation links and a short brand description, giving every page a clear, finished feel.
### Page-Specific Features
- **Home**: 
	- **Quick Facts Bar**: Four key breed stats — Size, Life Span, Energy Level and Temperament — give users an instant breed overview without having to read the full article.
	- **Breed Article**: A written section covering why Cocker Spaniels make great pets, accompanied by a real photograph of a Cocker Spaniel.
	- **Four Reasons Section**: A card-based section using emoji icons to highlight four characteristics of the breed, designed to give prospective owners an honest picture of what ownership looks like.
- **Care**:
	- **Grooming Cards**: Three cards summarising the key grooming commitments, giving prospective owners an instant understanding of what the breed's grooming requirements are.
	- **Feeding Guide**: A structured table breaking down recommended feeding portions from puppy through to senior.
	- **Pro Tips**: Highlighted pro tip boxes appear throughout the Care page to give important advice, visually distinct from the main content so they are easy to spot.
	- **Exercise Cards**: Four cards covering the key types of exercise a Cocker Spaniel needs, paired with an image of an exercising Cocker Spaniel.
- **History:**
	- **Origins Section**: An introductory written section covering the breed's roots and early history, accompanied by a quick facts table summarising key dates.
	- **Chronological Timeline**: The breed's history presented as a vertical timeline — easy to follow without overwhelming the reader.
	- **AKC Pull Quote**: A quote from the American Kennel Club sits between the timeline and breed types sections, adding a natural break between content.
	- **Breed Comparison Section**: A side-by-side comparison of the English, American and Working Cocker Spaniel, helping users understand the differences between the three breed types at a glance.
## Current Development

If you would like to see the features to be added in the future visit the Project board:
https://github.com/users/Hybrid965/projects/1/views/1

## Future Development
  - **Dynamic "Find a Rescue" Map**: Using an API integration such as Google Maps, I will add a feature allowing users to locate Cocker Spaniel rescue centres and clubs across the UK.
  - **Community Gallery**: I intend to build a gallery where owners can upload photos of their own Cocker Spaniels.
  - **Newsletter Sign-Up**: A simple sign-up form allowing users to receive breed tips and site updates.
## Testing

### HTML Validation

All three pages were tested using the [W3C Nu HTML Checker](https://validator.w3.org/).

| Page         | Errors / Warnings                                      | Validated Screenshot                                         |
| ------------ | ------------------------------------------------------ | ------------------------------------------------------------ |
| index.html   | No errors                                              | [Index validated](docs/testing/index.html-validated.png)     |
| care.html    | No errors / warnings                                   | [Care validated](docs/testing/care.html-validated.png)       |
| history.html | [History errors](docs/testing/history.html-errors.png) | [History validated](docs/testing/history.html-validated.png) |

During development, the history page returned the following errors which were subsequently fixed:

- **Article lacks heading** — resolved by moving the `<header>` element directly inside `<article id="timeline">`
- **Section lacks heading** — `<section id="quote">` changed to a `<div>` as no heading was needed
- **Missing `alt` attributes** — added `alt` text to all three breed images
- **Unclosed `<div>` element** — missing closing tag added in the breeds section

### CSS Validation

CSS was tested using the [W3C CSS Validator](https://jigsaw.w3.org/css-validator/).

| File         | Errors / Warnings                                   | Validated Screenshot                                  |
| ------------ | --------------------------------------------------- | ----------------------------------------------------- |
| index.html   | No errors                                           | [Index Css](docs/testing/index-css-validated.png)     |
| care.html    | [Care Css Errors](docs/testing/care-css-errors.png) | [Care Css](docs/testing/care-css-validated.png)       |
| history.html | No errors                                           | [History Css](docs/testing/history-css-validated.png) |

During development, `care-styles.css` returned the following warning which was subsequently fixed:

- **Same color for `background-color` and `color` on `body` (line 18)** — duplicate colour value removed

### Functional Testing

| Test                                   | Expected Result                       | Pass/Fail |
| -------------------------------------- | ------------------------------------- | --------- |
| Clicking logo in navbar                | Navigates to index.html               | Pass      |
| Clicking Home nav link                 | Navigates to index.html               | Pass      |
| Clicking Care nav link                 | Navigates to care.html                | Pass      |
| Clicking History nav link              | Navigates to history.html             | Pass      |
| Clicking Origins link in history hero  | Smooth scrolls to Origins section     | Pass      |
| Clicking Timeline link in history hero | Smooth scrolls to Timeline section    | Pass      |
| Clicking Breeds link in history hero   | Smooth scrolls to Breeds section      | Pass      |
| Clicking Grooming link in care hero    | Smooth scrolls to Grooming section    | Pass      |
| Clicking Nutrition link in care hero   | Smooth scrolls to Nutrition section   | Pass      |
| Clicking Exercise link in care hero    | Smooth scrolls to Exercise section    | Pass      |
| Footer Home link                       | Navigates to index.html               | Pass      |
| Footer Care link                       | Navigates to care.html                | Pass      |
| Footer History link                    | Smooth scrolls to top of history page | Pass      |
| Active nav link highlighted            | Current page link styled differently  | Pass      |

### Responsiveness Testing

| Device  | Navigation                               | Images                      | Pass/Fail                   | Evidence
| ------- | ---------------------------------------- | ----------------------------| --------------------------- | --------- 
| Desktop | Full navbar visible, all links displayed | Images display at full size | Pass                        |[Desktop](docs/testing/desktop-test.png)
| Tablet  | Full navbar visible, all links displayed | Images scale correctly      | Pass                        |[Tablet](docs/testing/tablet-test.png)
| Mobile  | Navbar stacks correctly                  | Images scale to full width  | Pass                        |[Mobile](docs/testing/mobile-test.png)

### Browser Testing

| Browser | Layout             | Navigation     | Images          | Pass/Fail | Evidence
| ------- | ------------------ | -------------- | --------------- | --------- |-----------
| Chrome  | Displays correctly | All links work | All images load | Pass      |[Chrome](docs/testing/desktop-browser-test-chrome.png)
| Edge    | Displays correctly | All links work | All images load | Pass      |[Edge](docs/testing/desktop-browser-test-edge.png)
| Firefox | Displays correctly | All links work | All images load | Pass      |[Firefox](docs/testing/desktop-browser-test-firefox.png)

### User Story Validation

|User Story | Evidence |
|-----------|----------|
|"As a prospective owner, I want to understand the grooming commitment| [Grooming Section](docs/story-validation/grooming-section.png)
|"As a prospective owner, I want to see key facts at a glance| [Quick Facts Bar](docs/story-validation/quick-facts-bar.png)
|"As a family owner, I want to understand the breed's energy levels so that I can plan appropriate exercise"| [Exercise Section](docs/story-validation/exercise-section.png)
|"As a prospective dog owner, I want to quickly understand the Cocker Spaniel's personality"| [Quick Facts Bar](docs/story-validation/quick-facts-bar.png)
|"As a parent, I want to know if Cocker Spaniels are good with children"| [Home Article](docs/story-validation/index-article.png)
|"As a first-time dog owner, I want clear and friendly information| [Four Reasons](docs/story-validation/four-reasons.png)
|"As a first-time owner, I want to understand how trainable the breed is| [Home Article](docs/story-validation/index-article.png)

### Current and Solved Bugs

| Bug | Solved? | How was it Solved | Date | Commit |
| --- | ------- | ----------------- | ---- | ------ |
| `Why Choose section` — margin on box causing overflow on mobile | Yes | Replaced margin/padding on `.margin` and `#choose-box-container` with smaller values in the 1000px media query | 10/03/26 | 11230b6 |
| `Why Choose section` — headings and boxes out of alignment on mobile | Yes | Removed `flex-grow: 3` from `.choose-box` and applied padding and margin to `.margin` and `#choose-box-container` in the 1000px media query | 10/03/26 | 11230b6 |
| `Article section` — image shrinking text when screen size reduces | Yes | Set `width: 50%` and `height: auto` on the image inside the 1000px media query | 09/03/26 | 38c5bdb |
| `Article section` — image not displaying at bottom below 1000px | Yes | Changed `order: -1` to `order: 1` on the image inside the 1000px media query | 09/03/26 | c05a1fb |
| `Hero section` — H1 overflowing below 1000px screen width | Yes | Added two media queries (720px and 600px) to reduce the hero heading font sizes | 13/03/26 | a33144c |
| `Mini Hero section` — after removing .hidden css style h2 has appeared — [H2 error](docs/testing/h2-error.png) | Yes | Heading was removed as it was no longer needed | 20/03/2026 | d39dc17 |
| `Article section` — image not stacking at bottom on mobile | Yes | Updated `#spaniel-article-container` to flex-direction: column and used order: 2 on image| 23/03/26|3865flf

## Deployment

### How was this site deployed?
This site was deployed to GitHub Pages using the following steps:

1. Navigate to the repository on GitHub
2. Click on the **Settings** tab
3. In the left sidebar, click on **Pages**
4. Under **Source**, select **Deploy from a branch**
5. Under **Branch**, select **main**
6. Click **Save**
7. The site was then published and accessible via the link `https://hybrid965.github.io/the-cocker-spaniel/`

### How can I clone this repository?
To run this project locally:

1. Navigate to the repository on GitHub
2. Click the green **Code** button
3. Copy the HTTPS URL
4. Open your terminal and run:
```
git clone https://github.com/Hybrid965/the-cocker-spaniel.git
```

## Credits

**Content**:

Favicon:
- Artist — https://www.flaticon.com/authors/maxim-kulikov

History Page:
- Gemini was used for the history timeline and facts about the Cocker Spaniel breed, cited here — [History facts](docs/credits/history-gemini-facts.pdf)
- Wikipedia was also used for finding content on the origins of Cocker Spaniels — https://en.wikipedia.org/wiki/Cocker_Spaniel
- The AKC quote was taken from the AKC website — https://www.akc.org/dog-breeds/cocker-spaniel/

**Media**: 
- All images were sourced from the developer's personal photographs.
- Icons for the breed types section were created by [Maxim Kulikov](https://www.flaticon.com/authors/maxim-kulikov)

**Code**:

Credits have been given in the source code where snippets have been taken from outside sources:
- Border collapse — https://www.w3schools.com/cssref/pr_border-collapse.php
- Nth child — https://www.w3schools.com/cssref/sel_nth-child.php
- Skip Link — https://www.w3schools.com/accessibility/accessibility_skip_links.php

**Fonts**: 
- Fonts were sourced from [Google Fonts](https://fonts.google.com/).


---