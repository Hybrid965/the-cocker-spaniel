## Purpose
**The Cocker Spaniel** is an informational website created for prospective dog owners who are researching breeds but are overwhelmed by lengthy, technical resources. The target audience is families and first-time dog owners who want a clear, friendly, and visually engaging introduction to the Cocker Spaniel breed before committing to ownership.

The site provides users with accessible information on the breed's temperament, exercise needs, grooming requirements, and suitability as a family pet. Rather than presenting dense text, the content is structured around the key questions a prospective owner would ask — is this breed right for my family? How much exercise do they need? How much grooming is involved?

The goal is that a new visitor can arrive at the site and within minutes have a clear, confident understanding of whether a Cocker Spaniel suits their lifestyle.
## User Stories
#### As a prospective owner:
- As a prospective dog owner, I want to quickly understand the Cocker Spaniel's personality so that I can decide if the breed suits my lifestyle.
- As a prospective owner, I want to see key facts at a glance so that I don't have to read lengthy text to get basic information.
- As a prospective owner, I want to understand the grooming commitment so that I can decide if I have the time and budget for the breed.

#### As a parent/family:
- As a parent, I want to know if Cocker Spaniels are good with children so that I can feel confident bringing one into my home.
- As a family owner, I want to understand the breed's energy levels so that I can plan appropriate exercise and activities.

#### As a first-time dog owner:
- As a first-time dog owner, I want clear and friendly information so that I don't feel overwhelmed by technical or medical jargon.
- As a first-time owner, I want to understand how trainable the breed is so that I know what to expect when bringing a puppy home.
## UX Design
#### Design Decisions
The site uses a warm, earthy colour palette to reflect the natural personality 
of the breed. Deep navy (#122c47) is used for the navigation and headings to 
provide strong contrast against lighter backgrounds. Playfair Display is used 
for headings and Lato for body text, keeping the site readable and friendly.
Deep navy (#122c47) is also used for headings, Brown (#8b4513) is used for sub headings and paragraphs use lighter brown (#7a6a58), 
The only exeption for this is the history page due to the background being (#f2e8d5)

All images include alt text to meet accessibility guidelines. Semantic HTML 
elements are used throughout to aid screen reader navigation.

#### Wireframes
📄 [Home](docs/wireframes/home.png)

📄 [Care](docs/wireframes/care.png)

📄 [History](docs/wireframes/history.png)

## Features
#### Navigation Bar
A fixed navigation bar sits at the top of the page with links to the Home, About and Contact sections. It allows users to quickly jump to any section of the site without scrolling, and is fully responsive across all screen sizes.

#### Hero Section
A full-width hero section greets the user with a bold headline and a short tagline describing the breed. A "Discover the Breed" button scrolls the user down to the main article section.

#### Quick Facts Bar
A snapshot bar displaying four key breed stats — Size, Life Span, Energy Level and Temperament. This allows users to get an overview of the breed at a glance without reading the full article.

#### Breed Article
A detailed written section covering why Cocker Spaniels make great pets, including their personality, exercise needs, grooming requirements and trainability. Accompanied by a photograph of a Cocker Spaniel.

#### Four Reasons Section
A card-based section highlighting four key characteristics of the breed — Family Companion, Active & Adventurous, High Maintenance, and Sensitive Soul. Each card uses an emoji icon for visual clarity.

#### Fully Responsive Design
The site is fully responsive across desktop, tablet and mobile screen sizes, with layout adjustments handled through CSS media queries to ensure a consistent user experience on all devices.

## Current Developement
If you would like to see the features to be added in the future visit the Project board:
https://github.com/users/Hybrid965/projects/1/views/1

## Testing
#### HTML Validation

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

#### CSS Validation

CSS was tested using the [W3C CSS Validator](https://jigsaw.w3.org/css-validator/).

| File         | Errors / Warnings                                   | Validated Screenshot                                  |
| ------------ | --------------------------------------------------- | ----------------------------------------------------- |
| index.html   | No errors                                           | [Index Css](docs/testing/index-css-validated.png)     |
| care.html    | [Care Css Errors](docs/testing/care-css-errors.png) | [Care Css](docs/testing/care-css-validated.png)       |
| history.html | No errors                                           | [History Css](docs/testing/history-css-validated.png) |
All stylesheets validated as **CSS Level 3 + SVG**. 

During development, `care-styles.css` returned the following warning which was subsequently fixed: 
- **Same color for `background-color` and `color` on `body` (line 18)** — duplicate colour value removed

#### Functional Testing

| Test                                   | Expected Result                       | Pass/Fail |
| -------------------------------------- | ------------------------------------- | --------- |
| Clicking logo in navbar                | Navigates to index.html               |           |
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

#### Responsiveness Testing

| Device  | Navigation                               | Layout                                  | Images                      | Pass/Fail |
| ------- | ---------------------------------------- | --------------------------------------- | --------------------------- | --------- |
| Desktop | Full navbar visible, all links displayed | Two-column layouts display side by side | Images display at full size | Pass      |
| Tablet  | Full navbar visible, all links displayed | Columns stack vertically                | Images scale correctly      | Pass      |
| Mobile  | Navbar stacks or collapses correctly     | Single column layout, no overflow       | Images scale to full width  | Pass      |

#### Browser Testing

| Browser | Layout | Navigation | Images | Pass/Fail |
|---------|--------|------------|--------|-----------|
| Chrome | Displays correctly | All links work | All images load | Pass |
| Firefox | Displays correctly | All links work | All images load | Pass |
| Edge | Displays correctly | All links work | All images load | Pass |

#### Current and Solved Bugs

| Bug                                                                                               | Solved? | How was it Solved                                                                                                                          | Date       | Commit  |
| ------------------------------------------------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | ------- |
| `Why Choose section` — margin on box causing overflow on mobile                                   | Yes     | Replaced margin/padding on `.margin` and `#choose-box-container` with smaller values in the 1000px media query                             | 10/03/26   | 11230b6 |
| `Why Choose section` — headings and boxes out of alignment on mobile                              | Yes     | Removed `flex-grow: 3` from `.choose-box` and applied padding and margin to `.margin` and `#choose-box-container`in the 1000px media query | 10/03/26   | 11230b6 |
| `Article section` — image shrinking text when screen size reduces                                 | Yes     | Set `width: 50%` and `height: auto` on the image inside the 1000px media query                                                             | 09/03/26   | 38c5bdb |
| `Article section` — image not displaying at bottom below 1000px                                   | Yes     | Changed `order: -1` to `order: 1` on the image inside the 1000px media query                                                               | 09/03/26   | c05a1fb |
| `Hero section` — H1 overflowing below 1000px screen width                                         | Yes     | Added two media queries (720px and 600px) to reduce the hero heading font sizes                                                            | 13/03/26   | a33144c |
| `Mini Hero section` - after removing .hidden css style h2 has appeared - [H2 error](docs/testing/h2-error.png) |         |                                                                                                                                            | 20/03/2026 |         |                                                          | 13/03/26 | a33144c |

## Deployment
#### How was this site deployed?
This site was deployed to GitHub Pages using the following steps:
1. Navigate to the repository on GitHub
2. Click on the **Settings** tab
3. In the left sidebar, click on **Pages**
4. Under **Source**, select **Deploy from a branch**
5. Under **Branch**, select **main**
6. Click **Save**
7. The site was then published and accessible via the link `https://hybrid965.github.io/the-cocker-spaniel/`
#### How can I clone this repository?
To run this project locally:
1. Navigate to the repository on GitHub
2. Click the green **Code** button
3. Copy the HTTPS URL
4. Open your terminal and run:

```
git clone https://github.com/Hybrid965/the-cocker-spaniel.git
```
## Credits

### Content
#### Fav icon
Artist - https://www.flaticon.com/authors/maxim-kulikov 
#### History page

Gemini was used for history timeline and facts about the cockerspaniel breed, cited here - [History facts](docs\credits\history-gemini-facts.pdf)

Wikipedia was also used for finding content on the origins of cockerspaniels -https://en.wikipedia.org/wiki/Cocker_Spaniel

The kennel club quote was taking from the AKC website -  https://www.akc.org/dog-breeds/cocker-spaniel/

### Media
Images used on this sourced via dev's personal photo's

Icons for the breed types section were created by [Maxim Kulikov](https://www.flaticon.com/authors/maxim-kulikov)
### Code
Credits have been given in the source code were snippets have been taken from outside sources:

Border collapse - https://www.w3schools.com/cssref/pr_border-collapse.php

Nth child - https://www.w3schools.com/cssref/sel_nth-child.php

### Fonts
Fonts were sourced from [Google Fonts](https://fonts.google.com/).

---
