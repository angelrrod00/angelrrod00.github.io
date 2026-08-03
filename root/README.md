# angel-rodriguez-site

Jekyll + Minimal Mistakes portfolio, configured for GitHub Pages.

## 1. Get it online (about 10 minutes)

1. Create a repository named exactly `YOURUSERNAME.github.io`.
2. Copy everything in this folder into the repo root and push to `main`.
3. Go to **Settings → Pages** and set the source to **Deploy from a branch → main → / (root)**.
4. Wait a minute or two. The site appears at `https://YOURUSERNAME.github.io`.

## 2. Replace the placeholders

Search the repo for `CHANGEME`. Every hit is in `_config.yml`:

| Field | What to put |
| --- | --- |
| `url` | `https://YOURUSERNAME.github.io` (no trailing slash) |
| `repository` | `YOURUSERNAME/YOURUSERNAME.github.io` |
| `author.links` → Email | your address |
| `author.links` → GitHub | your profile URL |
| `author.links` → LinkedIn | your profile URL, or delete the block |
| `author.location` | uncomment and fill, or leave commented out |

Then add `assets/images/profile.jpg` — that's the sidebar headshot. Without it you'll get a broken image, so either add the file or comment out the `avatar:` line.

## 3. Preview locally before pushing (recommended)

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`. Without this you're debugging by commit-and-wait, which gets old fast.

## Structure

```
_config.yml              site settings, author sidebar, defaults
_data/navigation.yml     top nav bar
index.md                 the About page (your homepage)
_pages/                  the four effort pages + archives + 404
_posts/                  one file per project, named YYYY-MM-DD-slug.md
assets/css/main.scss     small color/type overrides on top of the theme
assets/images/           profile photo, logo, post images
```

## Adding a project

Create `_posts/YYYY-MM-DD-some-slug.md`:

```yaml
---
title: "Project Name"
excerpt: "One sentence that shows up in the effort listing."
date: 2026-08-01
categories:
  - Engineering      # Music | Science | Engineering | Entrepreneurship
tags:
  - whatever
  - you want
---
```

Then the four sections: background and inspiration, process, result, where my head's at now.

**One category per post.** The permalink is `/:categories/:title/`, so a post filed under `Science` lives at `/science/its-title/`, nested under its effort page. Two categories would nest it twice. Use tags for everything else.

## Notes on this build

- Dates on the older posts are approximate — I set them from what you described so the archive sorts sensibly. Adjust the filename and the `date:` field together.
- The Trick or Heat post leaves out your note about authorship position. Your call, but it reads differently to a stranger than it does in a private draft.
- `MDC Wulfson` corrected to **Wolfson Campus**.
- The fusor post has a placeholder YouTube embed — swap `VIDEO_ID` or delete the block.
- `jekyll-archives` is **not** available on GitHub Pages, so this uses the theme's Liquid archives. Don't switch `category_archive.type` to `jekyll-archives` or the build fails.

## Later, when you want it

- **Threads:** add a `series:` field to front matter and list them on the effort page.
- **Custom domain:** add a `CNAME` file with your domain, then point DNS at GitHub. Nothing else changes.
- **Skins:** `minimal_mistakes_skin` in `_config.yml` — try `neon` or `dark` for the moodier version.
