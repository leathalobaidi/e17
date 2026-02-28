# Package Landing Page Generator
## How to use
1. Fill in every `[FIELD]` below — replace the brackets and placeholder text with your real answers
2. Copy the **entire file** (including the instruction section at the bottom)
3. Paste it into Claude and send — you'll get a complete, ready-to-use HTML landing page

---

## YOUR ANSWERS

**Q1 — Agency or business name**
`[e.g. E17Studios / BrightWeb / NorthBridge Digital]`

**Q2 — Package name**
`[e.g. The Genesis Package / The Starter Pack / The Pro Launch]`

**Q3 — One-line tagline** *(what the package delivers, in plain English)*
`[e.g. "Your complete digital foundation — website, logo, and 30 days of support"]`

**Q4 — Pricing**
- Sale price: `[e.g. £149]`
- Original / crossed-out price: `[e.g. £499]`
- Savings callout: `[e.g. "Save over £350 this October" — or leave blank to auto-calculate]`

**Q5 — Offer deadline** *(creates urgency banner — remove if no deadline)*
`[e.g. "October 31st" / "Friday 5pm" / "10 spots remaining"]`

**Q6 — Call-to-action destination**
`[e.g. mailto:hello@youragency.com / https://calendly.com/yourlink / https://yoursite.com/book]`

**Q7 — Design direction** *(pick one, or describe your own)*
- `[ ] Dark luxury` — deep black background, gold accents, serif headlines (like the Genesis example)
- `[ ] Light & clean` — white/cream background, bold sans-serif, minimal
- `[ ] Bold & colourful` — vibrant brand colour as background, high contrast, energetic
- `[ ] Custom:` `[describe your preferred colors, vibe, fonts]`

**Q8 — Package features** *(paste your bullet list — as many as you have)*
```
- [Feature 1, e.g. Up to 6 custom designed pages]
- [Feature 2, e.g. Mobile responsive on all devices]
- [Feature 3, e.g. WordPress CMS for full control]
- [Feature 4]
- [Feature 5]
- [add as many as needed]
```

**Q9 — Bonus / free items** *(things included at no extra cost — or write "none")*
```
- [e.g. FREE Logo Design Package (worth £200)]
- [e.g. 3 custom banner designs]
- [e.g. 3 business email accounts]
- [or: none]
```

**Q10 — FAQ** *(3–5 questions your customers commonly ask — or write "auto" to let Claude generate relevant ones)*
```
Q: [e.g. Is there a contract or lock-in?]
A: [e.g. No contract. You own everything delivered. No ongoing fees.]

Q: [e.g. How long does it take?]
A: [e.g. Most projects are delivered within 7–14 days.]

Q: [e.g. Do I need to provide content?]
A: [e.g. We can work with what you have, or help you write it.]

Q: [add more or delete — minimum 3 recommended]
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
