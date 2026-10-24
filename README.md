# The Adithya Journal

A vintage newspaper-inspired reading room collecting Adithya Bandara’s posts from Medium, Substack, Reddit, and LinkedIn.

## Run locally

No dependencies or build step required. With Python 3 installed:

```sh
python -m http.server 8000 
```

Open http://localhost:8000.

## Structure

- `index.html` — journal layout and metadata
- `styles.css` — responsive paper and dark themes
- `posts.js` — curated post collection
- `app.js` — filters, search, sorting, and theme controls
- `theme.js` — saved theme initialization before first paint
- `favicon.svg` — journal monogram

## Update posts

Add an entry to `window.JOURNAL_POSTS` in `posts.js` with `platform`, `title`, `url`, `date`, and `topic`. Supported platforms: Medium, Substack, Reddit, LinkedIn. Dates use `DD Mon YYYY`; leave unknown dates blank. Editor’s order follows the array. Newest/oldest sorting keeps undated entries last.

The collection is curated, not automatically synchronized. Articles open at the original publisher; full article text is not republished here.

## Deploy

Upload the contents of `` to any static host. All asset links are relative, including for hosting in a subdirectory. For GitHub Pages, use a static-site workflow or publish `` with your preferred deployment tool.

## Accessibility

Keyboard focus states, skip-to-posts link, reduced-motion support, live search counts, accessible platform toggles, and responsive layouts. Press `/` to search and Escape to clear the focused search. Theme preference is saved locally.

## Rights

Site content and branding belong to Adithya Bandara. Linked articles remain with their original publishers. No additional license is granted by this repository.
