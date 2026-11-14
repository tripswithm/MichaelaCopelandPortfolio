# Portfolio Website — GitHub Pages package

Exported from the Muse portfolio site on 2026-11-14 (updated export). This is the
published version, including the Corridian launch case study with its reposts
reel, the interactive Mayman mileage chart, the 40 Day Reset Instagram strip and
former-client label, the EnCharge AI former-client card, the reordered Case
Studies page (Mayman, Corridian, RTX, Lenovo), the new MY ROLE line, the new
Case Studies introduction, the consolidated Corridian metrics strip, the HAUS
ownership statement, Lenovo's actual pilot results leading its case study, the
corrected Sam Deneke title (President, Air & Space Defense Systems at Raytheon),
and the Pulse results graphic with the Success score section removed, and all
earlier content. Your phone number is not in this export.

## What's in here

- `index.html` — the whole site in one file (27 MB, all 137 images inlined).
  All 8 pages plus the Lenovo / EcoCAR / Johnson & Johnson / RTX rotation
  galleries are in this one file, reached by hash links (#/haus, #/rtx, etc.).
- `robots.txt` — allows all crawlers, including OpenAI's OAI-SearchBot
  (ChatGPT Search). Replace the placeholder sitemap URL with your real address.
- `sitemap.xml` — lists the one real URL. Hash sections can't be separate
  sitemap entries, but all their text is inside index.html, so a fetch of
  the page sees everything.
- `llms.txt` — a short plain-text summary of the site for AI tools.
- `.nojekyll` — tells GitHub Pages to serve the files as-is, without Jekyll.

## Publish it (no command line needed)

1. On GitHub, create a new **public** repository. Name it whatever you like,
   e.g. `portfolio`. (For a `tripswithm.github.io` address, name the repo
   exactly `tripswithm.github.io` instead.)
2. In the repo, click **Add file → Upload files**, and upload everything in
   this folder: `index.html`, `robots.txt`, `sitemap.xml`, `llms.txt`, `.nojekyll`.
   (If `.nojekyll` doesn't show in the upload, that's fine — GitHub sometimes
   hides dotfiles; the site still works without it.)
3. Before uploading, open `robots.txt` and `sitemap.xml` and replace
   `tripswithm.github.io/MichaelaCopelandPorfolio` with your real address:
   - Project repo: `https://tripswithm.github.io/portfolio/`
   - User site repo: `https://tripswithm.github.io/`
4. Go to the repo's **Settings → Pages**. Under "Build and deployment",
   choose **Deploy from a branch**, branch `main`, folder `/ (root)`, Save.
5. Wait a minute or two. GitHub will show your live URL at the top of the
   Pages settings. Open it and check the pages work.

## Help ChatGPT / Google find it

- **Fastest test:** paste your new GitHub Pages URL into ChatGPT and ask it
  about the portfolio. ChatGPT can fetch a public page when you give it the link.
- **Search discovery takes longer:** submit the URL in Google Search Console
  (search.google.com/search-console) and Bing Webmaster Tools, and submit the
  sitemap URL. Indexing typically takes days to weeks, and ChatGPT Search
  placement is never guaranteed — allowing OAI-SearchBot only makes the
  site eligible.
- **Training opt-out (optional):** if you want ChatGPT Search to cite the site
  but don't want OpenAI to crawl it for model training, add this to `robots.txt`:
  ```
  User-agent: GPTBot
  Disallow: /
  ```
  Search and training controls are independent.

## Things to know

- The site is one 27 MB file because every image is embedded in it. That is
  under GitHub's limits, but the first load is heavier than a normal site.
  If you want a faster, split-asset version later (separate image files),
  that needs a rebuild of the site into multiple files.
- Anyone with the GitHub Pages URL can open it, and the repo itself is public,
  so the files are downloadable from GitHub too. Don't put anything private
  in the repo.
- This export is a snapshot. Future edits in Muse won't update GitHub Pages
  automatically — export again and re-upload `index.html` when you change things.
- Your Muse public link keeps working independently of this. You don't have
  to choose one or the other.
