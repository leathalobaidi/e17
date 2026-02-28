# Package Landing Page Generator — FILLED EXAMPLE
## (Genesis Package — E17Studios)
## Copy everything below and paste into Claude

---

## YOUR ANSWERS

**Q1 — Agency or business name**
`E17Studios`

**Q2 — Package name**
`The Genesis Package`

**Q3 — One-line tagline**
`Your complete digital foundation — custom website, professional logo, CMS training and a full month of support`

**Q4 — Pricing**
- Sale price: `£149`
- Original / crossed-out price: `£499`
- Savings callout: `Save over £350 this October`

**Q5 — Offer deadline**
`October 31st`

**Q6 — Call-to-action destination**
`mailto:hello@e17studios.com?subject=Genesis Package Enquiry`

**Q7 — Design direction**
- `[x] Dark luxury` — deep black background, gold accents, serif headlines

**Q8 — Package features**
```
- Up to 6 Unique, Professionally Designed Pages (you can request more)
- Custom WordPress Development – modern, dynamic, and scalable
- Fully Mobile Responsive and optimized for all devices
- User-Friendly Navigation designed for better conversions
- Unlimited Revisions until 100% satisfied
- Content Management System (CMS) for full control
- Header & Footer Design + Interactive Sliding Banners
- FREE 3 Custom Banner Designs
- FREE 3 Professional Business Email Accounts
- 15 Industry-Relevant Stock Images
- Favicon Design & Hover Effects
- Google-Friendly Sitemap + Indexing
- W3C Certified HTML Code
- Dedicated Project Manager throughout your project
- Full Source Files + 100% Ownership Rights
- Completely Unique Design tailored to your brand
- 100% Satisfaction & Approval Assurance
- Social Media Integration (Facebook, Instagram, TikTok, YouTube)
- Payment Gateway Setup (PayPal, Stripe, or Bank Transfer)
- Booking Calendar Integration
- Google Maps Integration
- WhatsApp Chat Integration
- Custom Dynamic Forms (Contact, Registration, Inquiry)
- Newsletter Signup Area
- Google Analytics & Meta Pixel Setup
- Email Marketing Integration (Mailchimp or similar)
```

**Q9 — Bonus / free items**
```
- FREE Logo Design Package (3 original concepts by 2 dedicated designers — worth £200+)
- Full-Color & Grayscale logo versions
- Business Card Design
- Letterhead & Invoice Templates
- Email Signature & Footer Design
- App/Website Icon Design
- Delivered in all major formats: JPEG, PNG, PDF, PSD, AI
- 24–48 hour turnaround on initial logo drafts
- 1 Month FREE Maintenance & Support post-launch
```

**Q10 — FAQ**
```
Q: Is the £149 really the total price — no hidden fees?
A: Yes. £149 covers everything listed: website design, development, logo, CMS training and one month of support. No monthly fees, no setup costs, no surprises.

Q: How long does the project take?
A: Logo drafts are delivered within 24–48 hours. The full website build typically takes 7–14 days depending on content and revision rounds.

Q: Do I own the website when it's done?
A: Completely. You receive full source files and 100% ownership rights. The site, the code, the logo — all yours. Zero ongoing lock-in.

Q: What if I need more than 6 pages?
A: Not a problem — additional pages can be quoted transparently. The core package covers up to 6 pages, which is enough for most businesses.

Q: Does this include hosting and domain?
A: Hosting and domain are not included in the £149, but we guide you through choosing the right plan. Typical hosting costs £5–15/month.
```

---

## CLAUDE'S INSTRUCTION
*(Do not edit below this line — this is the task for Claude)*

---

You are an expert frontend developer and conversion copywriter. Using the answers provided above, build a **complete, single-file HTML landing page** for the package described.

### Requirements

**Structure — include all of these sections:**
1. Sticky nav — agency name left, CTA button right
2. Hero — package name as large headline, tagline, price reveal (sale vs original, savings badge), two CTAs (primary = claim offer, secondary = scroll to features), urgency deadline banner
3. Stats strip — 4 key numbers derived from the package (e.g. number of pages, revisions, turnaround, etc.)
4. Package overview — 4 cards summarising the main pillars of the package
5. Feature list — all features from Q8, split into two logical columns with numbered items
6. Integrations / tools section — infer relevant integrations from the features; display as chips
7. Bonus section — highlight everything from Q9; skip this section if Q9 is "none"
8. October/deadline offer banner — bold callout with the deadline from Q5; skip if no deadline given
9. Trust strip — 5 trust signals inferred from the package (e.g. "Unlimited Revisions", "100% Ownership", "Dedicated PM")
10. FAQ accordion — interactive expand/collapse, using answers from Q10 (or auto-generate if "auto")
11. Final CTA — full-width closing section with large price, headline, and primary CTA button
12. Footer — agency name, contact email, small print about the offer

**Design:**
- Apply the design direction from Q7 exactly
- Use Google Fonts — choose fonts that match the vibe (avoid Inter, Roboto, Arial)
- Use CSS custom properties (variables) for all colours and spacing
- All colours, shadows, animations must be consistent with the chosen direction
- Add scroll-reveal animations (IntersectionObserver) on all major sections
- Mobile responsive — works perfectly on 375px screens
- No external JS libraries — vanilla CSS + JS only

**Code quality:**
- Single self-contained `.html` file — all CSS and JS inline
- No placeholder images — use CSS shapes, emoji, or Unicode decorators instead
- All CTA buttons link to the destination from Q6
- Valid, semantic HTML5
- The page must feel **premium and conversion-focused**, not generic

**Output:**
Return ONLY the complete HTML file. No explanation, no markdown fences, no commentary before or after. Start with `<!DOCTYPE html>` and end with `</html>`.
