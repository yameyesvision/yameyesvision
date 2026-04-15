# Prompt for Claude -- YamEyes Vision Multi-Page Site Build

Copy everything below the line and paste it into your Claude conversation.

---

I need you to convert my current single-page website (yameyesvision.com) into a multi-page site. The current site is a single index.html file built with Tailwind CSS (CDN), Google Fonts (Newsreader + Manrope), and Material Symbols. Keep the exact same design language, color palette, typography, and visual style across all pages.

## Current Design System (do not change these)

- Background: #fcf9f4
- Dark sections: #1A2E27
- Accent/gold: #c28529
- Text primary: #1c1c19
- Text secondary: #424845
- Outline: #c2c8c4
- Headlines: Newsreader (serif)
- Body: Manrope (sans-serif)
- Icons: Material Symbols Outlined
- Tailwind via CDN with the existing custom config

## Pages to Build

Build each page as its own HTML file. Every page must include:
- The same fixed top nav bar (updated with links to all pages)
- The same footer
- A unique `<title>` tag (format: "Page Name | Adam Llamas -- YamEyes Vision")
- A unique `<meta name="description">` with a compelling 150-160 character description
- `<link rel="canonical">` pointing to its own URL
- Open Graph tags (og:title, og:description, og:image, og:url, og:site_name)
- Twitter Card tags (summary_large_image)
- JSON-LD structured data (specific schema types listed below for each page)
- Breadcrumb navigation below the top nav (with BreadcrumbList schema)
- One H1 per page
- Internal links to at least 2-3 other pages in the content body
- Mobile responsive

### 1. Homepage (index.html) -- REBUILD from current

Keep the current hero section, book preview, pull quote, reviews, about preview, music section, and email capture. But update:
- Nav links now point to separate pages: About (/about.html), The Book (/book.html), Music (/music.html), Services (/services.html), Blog (/blog.html), Press (/press.html), Contact (/contact.html)
- Add a "Stay Connected" link to /contact.html
- Add a brief "Latest from the Blog" section before the footer (placeholder for 3 blog post cards)
- Schema: WebSite (with site name and URL) + Person (Adam Llamas with sameAs links)
- Title: "Adam Llamas | To the Son Who Saved Me -- A Fatherhood Memoir"
- Meta description: "Adam Llamas is the author of To the Son Who Saved Me, a memoir about fatherhood, healing, and ten truths earned the hard way. Available on Amazon."

### 2. About Page (about.html)

Expand the current about section into a full page:
- Hero with author photo (author.png) and name
- Full bio in first person (use the existing bio text from the current site, expand it)
- A section called "Why YamEyes Vision" explaining the brand name and mission
- A timeline or journey section showing key life milestones (music, fatherhood, writing)
- CTA linking to the book page and contact page
- Schema: Person (full details, jobTitle: "Author", sameAs to all social profiles) + ProfilePage
- Title: "About Adam Llamas | Author, Father, Music Producer"
- Meta description: "Adam Llamas is the author of To the Son Who Saved Me. A father, musician, and storyteller writing from lived experience about fatherhood and healing."

### 3. Book Page (book.html)

Dedicated landing page for the memoir:
- Large book cover image (bookcover.jpg)
- Full synopsis (expand from current site text)
- "Ten Truths" section listing or previewing the chapter themes (use what you know from the site)
- All reader reviews from the current site, displayed prominently
- "Who This Book Is For" section (new dads, fathers healing from their own childhood, anyone navigating complicated family dynamics)
- Buy buttons: Amazon paperback + Kindle links (https://a.co/d/0gPBu3NL)
- Embedded book trailer video (https://youtu.be/KuI_i7G2P9g?si=zyOOD7DqR9G4qMcH)
- Embedded soundtrack link (https://youtu.be/0JgqYRMHMI8?si=_SBPpN5z_vJYMdYv)
- CTA to leave a review on Amazon
- Schema: Book (title, author, genre, bookFormat, offers with price $3.99, image, url) + AggregateRating (5 stars based on reviews shown) + individual Review entries
- Title: "To the Son Who Saved Me: Ten Truths for the Road Ahead | Adam Llamas"
- Meta description: "A deeply personal memoir about fatherhood, healing, and love. Ten truths earned the hard way. By Adam Llamas. Available in paperback and Kindle on Amazon."

### 4. Music Page (music.html)

Expand the current music section:
- Hero section with a music-themed heading
- Embedded YouTube videos (soundtrack + any other music content from the YamEyes Vision channel)
- Description of Adam's music background and style
- Link to Fiverr for custom work (https://www.fiverr.com/yameyesvision)
- CTA to the services page for custom projects
- Schema: MusicRecording (for the soundtrack, with name, creator, url) + MusicComposition
- Title: "Music by Adam Llamas | YamEyes Vision"
- Meta description: "Original music by Adam Llamas. Hear the soundtrack to To the Son Who Saved Me and explore music built around feeling and story."

### 5. Services Page (services.html)

New page for music production services:
- Heading: custom music production
- What Adam offers (original beats, scoring, custom music for projects)
- Who it's for (artists, content creators, filmmakers, brands)
- Process overview (inquiry, concept, production, delivery)
- Testimonials if available (or placeholder section)
- CTA button linking to Fiverr profile (https://www.fiverr.com/yameyesvision)
- Schema: Service (name, description, provider: Adam Llamas) + Offer
- Title: "Music Production Services | Adam Llamas -- YamEyes Vision"
- Meta description: "Custom music production by Adam Llamas. Original beats and compositions built around your story. Start a project on Fiverr."

### 6. Blog Page (blog.html)

Blog index/listing page:
- Heading: "Journal" or "Reflections" (fits the brand voice better than "Blog")
- Grid of blog post cards (placeholder 3-6 cards with titles, dates, short excerpts, "Read More" links)
- Placeholder post titles that match the brand themes:
  - "The Day Everything Changed"
  - "What My Son Taught Me About Showing Up"
  - "Why I Wrote This Book"
  - "Ten Truths: Where They Came From"
  - "Music, Fatherhood, and Finding My Voice"
  - "Breaking the Cycle"
- Each card links to a placeholder URL like /blog/post-title.html
- Schema: CollectionPage
- Title: "Reflections | Adam Llamas -- YamEyes Vision"
- Meta description: "Personal essays on fatherhood, healing, music, and growth by Adam Llamas. Real stories from a real life."

### 7. Press / Media Page (press.html)

- Heading: "Press & Media"
- Author bio section (short + long versions, marked as copy-ready)
- Downloadable headshot section (link to author.png)
- Book cover image (link to bookcover.jpg)
- "In the Media" section (placeholder for future press mentions, interviews, podcast appearances)
- Contact for media inquiries (link to contact page)
- Schema: Person (same as about page)
- Title: "Press & Media | Adam Llamas -- YamEyes Vision"
- Meta description: "Press resources for Adam Llamas, author of To the Son Who Saved Me. Download author photos, bios, and book cover images."

### 8. Contact Page (contact.html)

- Heading: "Get in Touch"
- Simple contact form (name, email, message) -- can be a static form that posts to MailerLite or Formspree
- Email address displayed (or a general inquiry note)
- Social media links (Instagram, YouTube, Pinterest) with icons
- For media inquiries, link to press page
- For custom music, link to services page
- Schema: ContactPage
- Title: "Contact Adam Llamas | YamEyes Vision"
- Meta description: "Reach out to Adam Llamas for media inquiries, collaborations, or to share your story. Connect on Instagram, YouTube, and Pinterest."

### 9. Privacy Policy (privacy.html)

- Standard privacy policy covering:
  - What data is collected (email via MailerLite signup, contact form submissions)
  - How data is used (newsletter, responding to inquiries)
  - Third-party services (MailerLite, Amazon affiliate links if any)
  - Cookie usage
  - User rights (unsubscribe, data deletion)
- Title: "Privacy Policy | YamEyes Vision"
- No schema needed

### 10. Terms of Service (terms.html)

- Standard terms covering:
  - Site usage
  - Intellectual property (book content, music, images)
  - External links disclaimer (Amazon, Fiverr, YouTube)
  - Limitation of liability
- Title: "Terms of Service | YamEyes Vision"
- No schema needed

## Navigation Structure

Update the nav bar across all pages:
- Logo/brand name "YamEyes Vision" links to /
- Links: About, The Book, Music, Services, Reflections (blog), Press, Contact
- Mobile hamburger menu with the same links
- Highlight the current page in the nav

## Footer (all pages)

Keep the current footer design but update:
- Privacy Policy link points to /privacy.html
- Terms link points to /terms.html
- Add a small nav with links to all main pages
- Keep social icons (Amazon, YouTube, Instagram, Pinterest)

## Important Rules

1. Keep the exact same visual design, colors, fonts, and feel as the current site
2. Every page must work on mobile
3. Use semantic HTML (header, main, section, article, footer, nav)
4. All images must have descriptive alt text
5. No JavaScript frameworks -- keep it simple HTML + Tailwind CDN + vanilla JS for mobile menu
6. All external links must have rel="noopener" and target="_blank"
7. Do not remove any existing content -- only reorganize it across pages and expand where noted
8. Keep the MailerLite email capture on the homepage and contact page
