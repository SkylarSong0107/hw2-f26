# Verification record

Checked September 27, 2026 against the assignment requirements, browser computed styles, and the 1200px reference screenshot. All 15 groups and their 46 individual assertions passed in a browser without extensions.

| Item | Result | Verified value |
| --- | --- | --- |
| 1. Stylesheets | Pass | `html5reset.css` loads before `style.css`. |
| 2. Favicon | Pass | `images/favicon.ico` resolves within the project site and returns HTTP 200. The handout's `/images/favicon.ico` would return HTTP 404 on this GitHub Pages project site. |
| 3. Body | Pass | Arial then Verdana; `#000000` background; `#ffffff` text; margins 20px top/right/left and 0 bottom. |
| 4. H1 | Pass | 42px, centered, 15px padding on every side. |
| 5. H2 | Pass | 30px and `#0d0d0d` by default. |
| 6. Paragraphs | Pass | 24px; 10px top/left padding, 0 right/bottom. |
| 7. Images | Pass | 250px CSS width, no CSS height, block display with equal auto side margins, 10px dashed white border. |
| 8. Divs | Pass | Minimum height 125px, 20px padding, 3px solid white border. |
| 9. Introduction | Pass | 15px radius, 15px top margin, 48px line height for 24px paragraph text. |
| 10. Red | Pass | `#ff0000`, right aligned, 50px left margin, 2px bottom and 5px left white borders. |
| 11. Blue | Pass | `#0000ff`, left aligned, 50px right margin, 5px right and 2px top white borders; heading and paragraph `#c4c4c4`. |
| 12. Yellow | Pass | `#ffff00`, right aligned, 50px left margin, 2px bottom and 5px left white borders; paragraph `#707070`. |
| 13. Green | Pass | Allowed `#008500`, left aligned, 50px right margin, 5px right and 2px top white borders. |
| 14. Footer | Pass | Gradient `#000000` 0%, `#0000ff` 25%, `#0066ff` 70%, `#000000` 100%; 5px solid white border. |
| 15. Footer paragraph | Pass | 20px, right aligned, 15px padding top/right/bottom and 0 left. |

Additional checks:

- The HTML body and `css/html5reset.css` match the course starter repository. All CSS color literals have six hexadecimal digits.
- The W3C CSS Validator reported 0 errors and 0 warnings. The Nu HTML validator reported 0 errors and 2 informational notes about self-closing elements in the unchanged starter HTML body.
- WAVE reported 0 errors, 0 contrast errors, and 0 alerts for the first published version. The revised version uses the same visual colors and will be rechecked after deployment.
- The page renders in Safari on the iPhone 15 Pro iOS 17.5 simulator. A Chrome extension injects one extra `div` after the footer; this produces an empty bordered area in Chrome only. The assignment handout explicitly warns about this extension behavior. The clean browser has five expected body `div` elements and no extra area.

The first published version was accepted by the user and submitted to Canvas. The autograder returned 75/100 and identified the font-family declaration and four colored-section border declarations. This branch uses explicit declarations for those five items. Autograder retesting awaits user review and deployment of this branch.
