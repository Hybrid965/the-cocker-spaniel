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
TBD

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
If you would like to see the features to be added in the future visit the Trello board:
https://trello.com/b/tJPEiuzM/the-cocker-spaniel

## Testing
#### Functionality Testing

| Test                                 | Expected Result                     | Pass/Fail |
| ------------------------------------ | ----------------------------------- | --------- |
| Clicking "Discover the Breed" button | Scrolls down to the article section | Pass      |
| Clicking Home nav link               |                                     |           |
| Clicking About nav link              |                                     |           |
| Clicking Contact nav link            |                                     |           |
| All external links open in new tab   |                                     |           |
#### Responsiveness Testing
| Device/Screen Size | Navigation | Layout | Images | Pass/Fail |
| ------------------ | ---------- | ------ | ------ | --------- |
| Desktop (1200px+)  |            |        |        |           |
| Tablet (768px)     |            |        |        |           |
| Mobile (375px)     |            |        |        |           |
#### Validation Testing
| File       | Validator        | Result                |
| ---------- | ---------------- | --------------------- |
| index.html | W3C Validator    | No Errors or Warnings |
| style.css  | Jigsaw Validator | No Errors or Warnings |

#### Browser Testing
| Browser | Pass/Fail |
| ------- | --------- |
| Chrome  |           |
| Firefox |           |
| Edge    |           |
#### Current and Solved Bugs  

| Bug                                                                                                                                     | Solved? | When     | Commit Code |
| --------------------------------------------------------------------------------------------------------------------------------------- | ------- | -------- | ----------- |
| `why choose section` - margin on why choose box causing overflowing on mobile                                                           | Yes     | 10/03/26 | 11230b6     |
| `why choose section` - Text out of alignment on mobile the headings and boxes are out of alignment compared to the rest of the document | Yes     | 10/03    | 11230b6     |
| `Article section` - Fix picture from shrinking text when screen size reduces                                                            | Yes     | 09/03/26 | 38c5bdb     |
| `Article Section` - Picture isn't displaying correctly, should be at the bottom of the article when screen size reduces below 1000px    | Yes     | 09/03/26 | c05a1fb     |
| `Hero Section` - H1 is overflowing when screenwidth is below 1000px                                                                     | No      |          |             |
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

#### Content
All written content on this site was written by Will Burkert.
#### Media
All images used on this sourced via personal photo's
#### Code
No external code snippets or libraries were used in this project.
#### Fonts
Fonts were sourced from [Google Fonts](https://fonts.google.com/).

---
