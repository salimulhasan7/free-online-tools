# Free Tools Website - WordPress Pack

A complete starter pack for a free online tools website: **10 working tools**
(HTML/CSS/JS, no backend needed) plus **10 SEO-optimized WordPress posts**.

```
wordpress-tools/
  content-plan.md          # Keyword research & growth strategy
  README.md                # This guide
  posts/                   # 10 WordPress-ready posts (paste into WordPress)
  tools/                   # 10 standalone tool files (also used for live preview)
```

## The 10 Tools

| Tool | Folder | Type |
|------|--------|------|
| Word & Character Counter | `tools/word-counter/` | Work |
| Strong Password Generator | `tools/password-generator/` | Work |
| Text Case Converter | `tools/case-converter/` | Work |
| Percentage Calculator | `tools/percentage-calculator/` | Work |
| Age Calculator | `tools/age-calculator/` | Work/Fun |
| Random Decision Maker | `tools/decision-maker/` | Fun |
| Morse Code Translator | `tools/morse-translator/` | Fun |
| Cool Username Generator | `tools/username-generator/` | Fun |
| Color Palette Generator | `tools/palette-generator/` | Work/Fun |
| Typing Speed Test | `tools/typing-test/` | Fun |

All tools run 100% in the browser. Nothing is uploaded to a server, so they
are private, fast, and cost you nothing to run.

## How to Add a Tool to WordPress (3 options)

### Option A - Custom HTML block (simplest, recommended)

1. Open each file in `posts/` (e.g. `posts/word-counter.html`).
2. At the top of the file is a settings block with the **Title, Slug,
   Meta description, Focus keyword, Category and Tags**.
3. Create a new Page in WordPress (Pages > Add New).
4. Add a **Custom HTML** block and paste everything from the line
   `PASTE FROM HERE` to the end of the file.
5. Set the Page slug (e.g. `word-counter`) in the page settings sidebar.
6. Install **Rank Math SEO** (free) and fill in the meta description and
   focus keyword from the settings block.
7. Publish. Done - the tool is live and styled so it does not clash with
   your theme.

### Option B - Upload the tool files and embed with an iframe

This keeps the tool completely isolated from your theme:

1. Upload each `tools/<name>/` folder to your server, e.g.
   `https://yoursite.com/wp-content/uploads/tools/word-counter/index.html`
   (use FTP or a file manager plugin).
2. In a WordPress post, add a Custom HTML block with:
   `<iframe src="https://yoursite.com/wp-content/uploads/tools/word-counter/index.html" style="width:100%;height:560px;border:0;border-radius:12px;"></iframe>`

### Option C - Shortcode (for developers)

Save the tool HTML as a snippet (e.g. with the free "Insert HTML Snippet"
plugin), then place its shortcode inside any post.

## Categories to Create

Create these categories before publishing so the posts link together nicely:

- **Work Tools**
  - Text Tools (word counter, case converter)
  - Calculators (percentage, age)
  - Generators (password, palette)
- **Fun Tools**
  - Random Generators (decision maker, username, morse)
  - Games (typing test)

## SEO Checklist (do for every page)

1. Title matches the post's `Title` in the settings block.
2. Slug matches the `Slug` in the settings block.
3. Meta description set in Rank Math (from the settings block).
4. Focus keyword set in Rank Math.
5. Featured image added (a screenshot of the tool works great).
6. FAQ `<details>` sections are already in each post - keep them, they can
   win Google featured snippets.
7. Every post already links to 3 related tools (internal linking - good SEO).

## Launch Order (from content-plan.md)

- **Week 1**: publish Work Tools (word counter, password generator, case
  converter, percentage calculator, age calculator).
- **Week 2**: publish Fun Tools (decision maker, morse, username, palette,
  typing test).
- **Week 3**: submit your sitemap to Google Search Console, then publish 3
  blog posts that link into the tools.

## Recommended Plugins

- **Rank Math SEO** (free) - titles, descriptions, sitemap, schema
- **LiteSpeed Cache** or **WP Rocket** - page speed
- **Table of Contents Plus** - adds a TOC to tool pages

## Monetization (later, see content-plan.md)

- AdSense/Ezoic/Mediavine after traffic grows
- Affiliate links: hosting, keyboards, design tools
- Newsletter capture on the word counter and typing test pages
