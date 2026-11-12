# Website / CRO audit

**URL:** https://cityglassukltd.co.uk/  
**Observed:** 2026-08-29  
**Evidence:** `website_desktop_1440x900.png`, `website_mobile_390x844.png`, and `squirrel_surface_audit.llm.txt` in this directory.

## Method and scope

- Real headless Google Chrome captures: 1440×900 desktop and 390×844 mobile. They show the public page as rendered at capture time; neither capture submits a form or logs in.
- Bounded Squirrel surface audit: 20 pages, capped at 20, run in this directory. It reported overall 46/100. This is diagnostic evidence, not a customer-facing grade, a promise of search performance, or the sole purchase rationale.
- The Squirrel command auto-updated itself from v0.0.86 to v0.0.87 before scanning. This was an unexpected local tool mutation; no project files outside this research directory were intentionally changed. Its result remains usable as an audit record, with that provenance caveat.

## Rendered customer journey observations

| Area | Desktop 1440×900 | Mobile 390×844 | Commercial implication |
|---|---|---|---|
| Hero | Recognisable branded vehicles, but a very pale overlay washes down the visual proof and the headline/CTA are effectively below the cookie banner in this capture | Same vehicle image dominates; consent interface covers a large portion of the initial viewport | First visit should identify the jobs and route to a quote before nonessential choice overload. |
| Navigation | Broad service navigation is visible (windows, doors, balustrades, cupolas, splashbacks, repairs, more) | top line contains social icons and an email string that is visually truncated; the menu action is not meaningfully available within this capture | Make the first three choices explicit rather than relying on a long menu. |
| Trust | Real branded fleet is valuable proof; Trusted Trader is linked | cookie layer blocks the early journey | Bring verified local proof and contact intent nearer to the key service choices. |
| CTA | “Email Us” exists but initial quote intent is visually subordinated | the consent view pushes meaningful action below the fold | A static concept can present one high-intent “Request a quote / survey” route to the existing contact page; it must not claim to submit enquiries. |
| Services | Website covers many relevant services | detail is not visible before consent / fold | Select a truthful, small core slice; do not flatten all services into generic “glazing”. |

## Information architecture observed

Home navigation exposes `Windows`, `Doors`, `Balustrades`, `Cupolas`, `Splashbacks`, `Glass Repair`, `More`, plus a separate contact page. The web surface has at least 33 sitemap URLs according to the audit crawl. This breadth is useful for organic detail pages but creates a different first-visit problem: users must infer which route fits their job before seeing concise local proof and one enquiry option.

## Bounded technical findings (not the principal sales message)

- Surface audit: 46/100 overall; 20 pages crawled; WordPress/Divi, LiteSpeed, CookieYes, Google Fonts and jQuery detected.
- The audit flags disabled viewport zoom on sampled pages, missing accessible names, absent iframe title on contact, some missing alt text, multiple H1s on sampled pages and lengthy/blocking scripts. It also reports metadata/schema/image and security-header issues.
- It reports a `/services/` URL as a 404. This is a concrete navigation/content opportunity only if the link is actually exposed to visitors; the current concept proposal does not rely on it.
- One LinkedIn external-link result is marked status 999 by the scanner. That can be a remote-platform scan limitation, so it is **not** called a customer-visible broken link without independent browser confirmation.

## Priority interpretation

The recommended £600 concept should **not** lead with “your SEO/security/accessibility is poor.” Those issues are implementation audit findings. The honest commercial proposition is a clearer, more confident entry page for real service categories, real Edinburgh/Lothian coverage and existing quote intent.

## No-interaction boundary

No cookie consent button was pressed, no form was completed, no call/email link was activated, no social account was opened and no backend route was accessed.
