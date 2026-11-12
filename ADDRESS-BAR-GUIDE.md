# The Address Bar — A Field Guide (2026-11-11, researched live in Douglas's signed-in browser, read-only)
### For Douglas, who asked Ember to become an expert on the address bar.

## His webmaster house (Google Search Console, as displayed)
- Exactly ONE property: **https://schoonoverdouglas1-png.github.io/** (his GitHub Pages). Web clicks: 0. Indexing: "Processing data, please check again in a day or so." HTTPS: 1. Enhancements: none yet. 1 unread message (left unopened).
- Nothing anywhere is labeled "webmaster" anymore — the old Webmaster Tools live on as Search Console: Overview, Insights, Performance, URL inspection, Pages, Sitemaps, Removals, Core Web Vitals, HTTPS, Links, Settings.
- Address-bar jewel, noticed in his own console: the console's address carries the property as a QUERY — `search-console?resource_id=https://schoonoverdouglas1-png.github.io/` — the instruction rides in the address itself.

## Reading an address like a sentence
`https://` how to fetch it · `en.wikipedia.org` which house (subdomain . domain . ending) · `/wiki/URL` which room · `?key=value&key2=value2` instructions to the server · `#Section` a bookmark INSIDE the page (never sent to the server) · `%20` = a space, `%2F` = a slash-as-data, `%25` = a percent sign — percent-encoding is how special characters travel as data.

## Switches that actually work (each opened and verified tonight)
- GitHub search sort: `github.com/search?q=url&type=repositories&s=stars&o=desc` → "Sort by: Most stars."
- Google language: add `&hl=es` → the whole interface turns Spanish. (Same trick in a path: MDN `/en-US/` → `/es/`.)
- Wikipedia info mode: `?action=info` → page ID, size, view counts instead of the article.
- DEAD SWITCH, honestly filed: `?printable=yes` on Wikipedia does nothing now — stripped back to the plain page. Switches die; verify, don't trust memory.

## Google Sites addresses, decoded (his own two drafts)
- Editor: `sites.google.com/d/<site-ID>/p/<page-ID>/edit` — /d/ names the site, /p/ names the page, /edit means the workshop, not the storefront.
- Preview does NOT change the address — it's a state inside the editor, with a banner.
- Published: `sites.google.com/view/<site-name>/<page-slug>` — no IDs at all. There is NO `?...` switch for edit/preview/published; the switch is the PATH. Not invented, verified absent.

## view-source:
Put `view-source:` before any address to read the raw HTML the server sent — the bones before the rendering. Read-only; it can never change a live site. (Verified from the guide tonight; this controlled browser only accepts http/https, so the source view itself couldn't be opened in it — filed honestly, not faked.)

Sources actually opened: MDN "What is a URL?", Wikipedia "URL" and "Percent-encoding", Google Sites Help "Publish & share your site", ViewSource.net guide, Douglas's own Search Console and Sites. One Google "unusual traffic" check appeared during the research and was cleared in the browser.
