SumBuck sb.lumbermen.org preview fix

This package keeps the visual appearance of the marketing page intact while making the HTML lighter for link-preview bots and crawlers.

Changes made:
- Extracted 5 large inline base64 JPEG images from index.html into normal files under /assets/.
- Updated CSS and img references to use those external files.
- Changed the Open Graph/Twitter preview image URL to /og-sumbuck-v2.jpg to force services to fetch a fresh image.
- Kept /og-sumbuck.jpg and added /og-sumbuck-v2.jpg.
- Added a lightweight /share/ page with the same preview metadata as a fallback sharing URL.
- Kept the visible design and body copy essentially intact.

Deploy all files and folders in this package to the root of the sb.lumbermen.org site.

After deploying, test:
https://sb.lumbermen.org/og-sumbuck-v2.jpg
https://sb.lumbermen.org/share/
https://sb.lumbermen.org/?fresh=1

For iMessage, test by sending one URL by itself in a fresh thread:
https://sb.lumbermen.org/?fresh=1

If the root URL still shows a cached preview, use:
https://sb.lumbermen.org/share/

