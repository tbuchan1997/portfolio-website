#Portfolio Website

# Software Developer Portfolio Website

## User Stories

### Must Haves
- **As a visitor, I want to see the developer's name and a short introduction** so that I know who they are.
- **As a visitor, I want to navigate to different sections of the portfolio (About, Projects, Contact)** so that I can easily explore their work.
- **As a visitor, I want to view a list of the developer's projects** so that I can see examples of their work.
- **As a visitor, I want to access contact information or a contact form** so that I can reach out to the developer.
- **As a visitor, I want the website to be responsive** so that I can view it on different devices.

### Should Haves
- **As a visitor, I want to see a list of technical skills and proficiencies** so that I can assess the developer's expertise.
- **As a visitor, I want to view project details, such as descriptions, technologies used, and links to live demos or GitHub repos** so that I can evaluate their work.
- **As a visitor, I want smooth scrolling navigation** so that I have a better user experience.
- **As a visitor, I want links to the developer's professional profiles (e.g., LinkedIn, GitHub)** so that I can learn more about their professional background.

### Can Haves
- **As a visitor, I want to see animations or visual effects (e.g., hover effects, transitions)** so that the website feels modern and interactive.
- **As a visitor, I want a dark mode toggle** so that I can choose the theme I prefer.
- **As a visitor, I want to download the developer's resume** so that I have access to their detailed qualifications.
- **As a visitor, I want testimonials from colleagues or clients** so that I can see feedback on the developer's work.
- **As a visitor, I want a blog or insights section** so that I can learn more about their thoughts and experiences in software development.

---

## Development Process

### Step 1: Develop the HTML

#### Action-Based To-Do's
1. **Set up the structure:**
   - Create an `index.html` file and add a basic HTML5 boilerplate.
   - Add `<header>`, `<main>`, `<footer>` tags.
   - Include `<section>` elements for About, Projects, and Contact sections.

2. **Add content for each section:**
   - **About Section:**
     - Write a brief introduction inside a `<p>` tag.
     - List technical skills using `<ul>` or `<dl>` for organization.
   - **Projects Section:**
     - Add a grid or list with `<article>` elements for each project.
     - Include `<img>` for project thumbnails, `<h3>` for titles, `<p>` for descriptions, and `<a>` for links to live demos/repositories.
   - **Contact Section:**
     - Use a `<form>` element with `<input>` fields for name and email, a `<textarea>` for messages, and a `<button>` for submission.
     - Add clickable icons (e.g., `<a>` wrapping `<i>` or `<svg>`) for social media.

3. **Ensure accessibility:**
   - Add `alt` attributes for all images.
   - Label form fields using `<label>` elements or `aria-label`.

#### Success Criteria
- The page has all necessary sections and content structured semantically.
- All images include descriptive `alt` text.
- Navigation links work and jump to the correct section when clicked.

---

### Step 2: Style with CSS

#### Action-Based To-Do's
1. **Set up a responsive layout:**
   - Use CSS Grid or Flexbox to position header, main sections, and footer.
   - Write media queries for breakpoints (e.g., mobile-first design).
     - Define a single-column layout for small screens.
     - Switch to a multi-column layout for larger screens.

2. **Apply visual design:**
   - Define CSS variables for colors and typography.
   - Style headings, paragraphs, and lists for readability.
   - Add hover effects to buttons and links with `:hover` and `:focus` pseudo-classes.

3. **Enhance accessibility and readability:**
   - Test color contrast using online tools (e.g., WCAG contrast checker).
   - Add consistent padding/margin for uniform spacing.
   - Use `rem` units for scalable typography.

4. **Optional Animations:**
   - Use `transition` for smooth hover effects.
   - Add `scroll-behavior: smooth;` to the `html` tag for smooth scrolling.

#### Success Criteria
- The website looks visually appealing and organized on desktop and mobile devices.
- Navigation and buttons respond to hover and focus states.
- Spacing and typography are consistent across all sections.
- Animations enhance the experience without being distracting.

---

### Step 3: Add JavaScript Functionality

#### Action-Based To-Do's
1. **Must-Have Features:**
   - **Navigation Scrolling:**
     - Add `id` attributes to section headers (e.g., `id="about"`) for anchor points.
     - Add `eventListeners` to navigation links for smooth scrolling using JavaScript's `scrollIntoView` method.
   - **Form Validation:**
     - Check for empty fields and validate the email field with a regular expression.
     - Show error messages below invalid inputs.

2. **Should-Have Features:**
   - **Dynamic Project Cards:**
     - Create a `projects.json` file containing project data (title, description, image, links).
     - Fetch the data using `fetch()` and dynamically create project cards using `document.createElement()`.

   - **Sticky Header:**
     - Use CSS `position: sticky` or JavaScript to make the header stick to the top when scrolling.

3. **Can-Have Features:**
   - **Dark Mode Toggle:**
     - Add a toggle button in the header.
     - Use JavaScript to toggle a `dark-mode` class on the `<body>` element.
     - Save the user’s preference in `localStorage`.

   - **Interactive Animations:**
     - Use JavaScript libraries (e.g., GSAP) for scroll-triggered animations.
     - Add tooltips to social media icons on hover.

#### Success Criteria
- **Must-Have:** Navigation links smoothly scroll to the correct section. The form validates inputs and shows error messages for invalid fields.
- **Should-Have:** Projects load dynamically from JSON. The header stays visible while scrolling.
- **Can-Have:** Dark mode toggles correctly and remembers the user's preference. Animations and tooltips improve interactivity.

---

### Must-Have: Navigation Scrolling
**To-Do:**
- Add `eventListener` for all navigation links.
- Use `scrollIntoView` for smooth scrolling.

**Success Criteria:**
- Clicking a navigation link smoothly scrolls to the target section.

### Can-Have: Dark Mode
**To-Do:**
- Create a button for toggling dark mode.
- Toggle a `dark-mode` class on the `<body>` and save the state in `localStorage`.

**Success Criteria:**
- The site switches themes when toggled, and the chosen theme persists across sessions.
