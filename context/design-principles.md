# S-Tier Design Principles & Quality Standards

> Combined from Patrick Ellis's design system (Stripe, Airbnb, Linear standards) and Aftermark AI's anti-vibe-coded research across 500+ websites.

## I. Core Design Philosophy

### Guiding Principles
- **Users First:** Prioritize user needs, workflows, and ease of use in every design decision
- **Meticulous Craft:** Aim for precision, polish, and high quality in every UI element
- **Speed & Performance:** Design for fast load times and snappy, responsive interactions
- **Simplicity & Clarity:** Strive for a clean, uncluttered interface with unambiguous communication
- **Consistency:** Maintain a uniform design language across the entire application
- **Accessibility (WCAG AA+):** Design for inclusivity with sufficient contrast and keyboard navigability

---

## II. Design System Foundation

### Color Palette
- [ ] **Primary Brand Color:** User-specified, used strategically (not everywhere)
- [ ] **Neutrals:** A scale of grays (5-7 steps) for text, backgrounds, borders
- [ ] **Semantic Colors:** Success (green), Error (red), Warning (amber), Info (blue)
- [ ] **Dark Mode:** Create corresponding accessible dark mode palette
- [ ] **Contrast Check:** All combinations meet WCAG AA (4.5:1 minimum)

### Typography Scale
- [ ] **Primary Font:** Clean, legible sans-serif (Inter, Manrope, system-ui)
- [ ] **Modular Scale:** Distinct sizes for H1, H2, H3, H4, Body, Caption
- [ ] **Font Weights:** Limited set (Regular, Medium, SemiBold, Bold)
- [ ] **Line Height:** Generous for readability (1.5-1.7 for body text)
- [ ] **Consistency:** Same typography treatment across all pages

### Spacing System
- [ ] **Base Unit:** Establish 4px or 8px base
- [ ] **Spacing Scale:** Use multiples only (4, 8, 12, 16, 24, 32, 48, 64)
- [ ] **No Magic Numbers:** Every spacing value comes from the scale
- [ ] **Consistent Rhythm:** Predictable spacing creates polish

### Border Radius
- [ ] **Small:** 4-6px for inputs, buttons
- [ ] **Medium:** 8-12px for cards, modals
- [ ] **Large:** 16-24px for prominent containers
- [ ] **Consistency:** Same radius for same component types everywhere

---

## III. Component Standards

### All Components Must Have
- [ ] Default state
- [ ] Hover state (subtle, not aggressive)
- [ ] Active/pressed state
- [ ] Focus state (visible for accessibility)
- [ ] Disabled state
- [ ] Loading state (where applicable)
- [ ] Error state (where applicable)

### Buttons
- [ ] Primary, secondary, tertiary/ghost, destructive variants
- [ ] Consistent padding and height
- [ ] Icon support (left or right)
- [ ] Loading spinner integration
- [ ] No bouncing or aggressive animations

### Form Inputs
- [ ] Clear labels (not just placeholders)
- [ ] Helper text support
- [ ] Error message display
- [ ] Consistent height with buttons
- [ ] Proper focus rings

### Cards
- [ ] Consistent padding
- [ ] Subtle shadow (not flashlight-under-mouse effect)
- [ ] Hover lift of 2-4px maximum (if any)
- [ ] No rotation on hover

### Navigation
- [ ] Clear active state indication
- [ ] Logical grouping
- [ ] Mobile-responsive behavior
- [ ] No transparency issues with scrolling content

---

## IV. Interaction & Animation Standards

### Animation Principles
- [ ] **Duration:** 150-300ms for micro-interactions
- [ ] **Easing:** Use ease-in-out or custom bezier curves
- [ ] **Purpose:** Every animation serves a purpose (feedback, guidance)
- [ ] **Subtlety:** If you notice the animation first, it's too much

### What to Animate
- [ ] State transitions (hover, focus, active)
- [ ] Page/section transitions
- [ ] Loading indicators
- [ ] Success/error feedback
- [ ] Content appearing (fade-in, not bounce)

### What NOT to Animate
- [ ] Cards rotating on hover
- [ ] Aggressive lift effects
- [ ] Wiggle or bounce effects
- [ ] Scroll-triggered animations that stutter
- [ ] Decorative Lottie animations that don't match brand

### Loading States (Critical)
- [ ] **Buttons:** Show spinner or loading text during async actions
- [ ] **Pages:** Use skeleton screens, not empty white space
- [ ] **Lists:** Show skeleton items while loading
- [ ] **Forms:** Disable submit and show progress

---

## V. Layout Standards

### Grid System
- [ ] Use 12-column responsive grid
- [ ] Consistent gutters (16px or 24px)
- [ ] Proper alignment at all breakpoints
- [ ] No elements drifting out of alignment

### Responsive Breakpoints
- [ ] Mobile: 375px (primary design target)
- [ ] Tablet: 768px
- [ ] Desktop: 1024px
- [ ] Large Desktop: 1440px

### Spacing Rhythm
- [ ] Section spacing consistent throughout
- [ ] Component spacing predictable
- [ ] No random margins or padding
- [ ] Visual balance and breathing room

### Visual Hierarchy
- [ ] Clear primary action on each screen
- [ ] Typography guides the eye
- [ ] Proper contrast between elements
- [ ] White space used intentionally

---

## VI. Content & Copy Standards

### Headlines & Taglines
- [ ] Specific value proposition (not "Build your dreams")
- [ ] Clear what the product does
- [ ] Speaks to user benefit
- [ ] No buzzword stacking

### Microcopy
- [ ] Button labels are action-oriented ("Save Changes" not "Submit")
- [ ] Error messages explain how to fix
- [ ] Empty states guide next action
- [ ] Loading text is contextual

### Footer & Legal
- [ ] Copyright text is correct (not "All right reversed")
- [ ] Year is current
- [ ] Links are functional
- [ ] Professional tone

### Testimonials (if used)
- [ ] Real names with context (job title, company)
- [ ] Specific quotes (not "Helped me so much")
- [ ] Real photos (not AI-generated faces)
- [ ] Links to verify if possible

---

## VII. Technical Quality Standards

### Meta & SEO
- [ ] Proper page titles (not "Home" or "Untitled")
- [ ] Meta descriptions written
- [ ] OpenGraph image configured
- [ ] Favicon present

### Performance
- [ ] Images optimized (WebP, proper sizing)
- [ ] Lazy loading for below-fold content
- [ ] No layout shift (CLS)
- [ ] Fast initial load (<3s)

### Functionality
- [ ] All buttons do something
- [ ] All links go somewhere real (not "#")
- [ ] Social icons link to actual profiles
- [ ] Forms submit and provide feedback
- [ ] Dark mode toggle works (if present)

### Console Health
- [ ] No JavaScript errors
- [ ] No 404 resources
- [ ] No mixed content warnings
- [ ] Clean console in production

---

## VIII. Pre-Ship Checklist

### Visual Polish
- [ ] No purple gradients (unless brand-specified)
- [ ] Sparkle usage minimal (0-1 per page)
- [ ] Consistent border radius throughout
- [ ] Typography hierarchy clear
- [ ] Color palette disciplined

### Responsiveness
- [ ] Mobile layout works perfectly
- [ ] Tablet layout adapts appropriately
- [ ] No horizontal scroll
- [ ] Touch targets 44px minimum
- [ ] Text readable without zooming

### Functionality
- [ ] All interactive elements work
- [ ] Loading states present
- [ ] Error states handled
- [ ] Empty states designed
- [ ] Forms validate properly

### Accessibility
- [ ] Keyboard navigation works
- [ ] Focus states visible
- [ ] Color contrast passes
- [ ] Images have alt text
- [ ] ARIA labels where needed

### Performance
- [ ] Page loads quickly
- [ ] No layout shift
- [ ] Images optimized
- [ ] Animations smooth

---

## IX. Vibe-Coded Energy Detector

**If 5+ of these are true, your site looks vibe-coded:**

### Visual Red Flags
- [ ] Purple gradient hero section
- [ ] Sparkle emoji/icon everywhere
- [ ] Hover animations on every card
- [ ] Emojis as UI elements
- [ ] Fake testimonials with AI faces
- [ ] Social icons that go nowhere
- [ ] Massive icons with tiny text
- [ ] Semi-transparent header with blur issues

### Structural Red Flags
- [ ] No loading states
- [ ] Inconsistent component placement
- [ ] Misaligned grids
- [ ] Different border radiuses everywhere
- [ ] Buttons/cards that bounce aggressively

### Content Red Flags
- [ ] "Build your dreams" type taglines
- [ ] Copyright typos
- [ ] Placeholder text left in
- [ ] Generic "Sarah P." testimonials

### Technical Red Flags
- [ ] Missing OG image
- [ ] No favicon
- [ ] Non-functional interactive elements
- [ ] Broken mobile layout
- [ ] Console errors

---

*This document should be referenced before, during, and after every UI implementation.*
