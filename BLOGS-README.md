Suck N' Shine Journal structure
===============================

SEO-priority articles are deliberately hardcoded as standalone HTML:
- blog-affordable-monthly-car-cleaning.html
- blog-10-things-in-your-car.html

The Journal index is:
- blog.html

Future/lightweight articles can be added to blogs.json.
Set "published": true to make a JSON article appear automatically on blog.html.
The Journal will link it to blog-post.html?slug=YOUR-SLUG.

Supported section fields in blogs.json:
- label
- heading
- paragraphs: []
- list: []
- callout

The example item in blogs.json is unpublished and will not appear on the live Journal until published is changed to true.

Important: JSON loading requires the site to be served over HTTP/HTTPS (Cloudflare Pages is fine). Some browsers block fetch() when opening the HTML directly from file://.
