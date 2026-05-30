# QA — Васил Атанасов

Status: local build ready for deploy.

## Gates

1. Source/fact audit — PASS
- Name/category/address/phone/place_id/CID/hours/social/testimonials/images documented in `image-map.md`.
- No prices, credentials, awards, guarantees, or review counts in public copy/schema.

2. Visual-result image audit — PASS
- Rechecked Oink raw HTML, MyBulgariaCenter/Google images, Maps image resources, ReviewEuro, BeautyNailHairSalons mirror, Yahoo/DDG/Bing, Facebook normal/mobile/mbasic/photo routes, Instagram/Studio24/Fresha search notes.
- Found 1 clean real final-result photo + 1 real styling/action photo; used near top.

3. Testimonial audit — PASS
- Named ReviewEuro testimonial text available and used as short excerpts with original names/language: Konstansa, Румяна, Latinka, Sofia.
- Google Maps profile link uses CID: `https://www.google.com/maps?cid=12826440804543399623`.

4. Copy audit — PASS
- Bulgarian copy checked for natural phrasing; no internal research/source mechanics in visible copy.

5. Links/schema/SEO head — PASS local
- Required title/meta/robots/canonical/OG/twitter present.
- One H1.
- HairSalon schema includes NAP, geo, opening hours, sameAs, image, canonical URL.

6. Image/layout audit — PASS local static inspection
- Selected images load from local `assets/`.
- Final result image uses portrait frame; action/interior images use gallery frames.
- One deliberate reuse of `result-bob.webp` (hero + first gallery) because it is the only clean final-result photo; documented in image-map.

7. Map/local SEO audit — PASS local
- Bottom map block directly above footer.
- Exactly one visible Google Maps navigation CTA in the map block.
- Iframe uses business name + full address query.

8. Responsive visual QA — LIMITED PASS
- Browser/screenshot tool unavailable in this subagent environment; static responsive CSS and local HTML/assets inspected. No automated screenshot was captured.

9. Final live QA — PASS
- Live URL: `https://deanooooooooo.github.io/vasil-atanasov-site/`
- HTTP 200 verified after Pages build.
- Live HTML contains business name, testimonial name `Konstansa`, HairSalon schema, canonical, OG image, and map iframe query.

## 2026-05-30 image-quality correction
- Replaced weak street/back-view hero with strongest vetted candidate.
- Removed weak action/interior filler images from visible use.
- Final visible image set reduced to the strongest hero only; no duplicate visible image srcs.
- Map iframe changed to eager load for better visual QA.
