# Avalon Chronicles 🏰

A personal blog with a medieval manuscript aesthetic — parchment textures, illuminated first letters, and a hand-drawn willow tree. Built with plain HTML/CSS/JS and Firebase (Firestore) for content, deployed on Netlify.

## Pages

- `index.html` — home page, shows the 3 most recent posts
- `blogs.html` — full archive, filterable by language and type (essay / review / poetry)
- `blog.html` — single post view (`blog.html?slug=your-slug`)
- `about.html` — about page, EN/TR toggle
- `ayseyagmur.html` — content admin panel (add / edit / delete posts)

## Tech

- Static HTML/CSS/JS, no build step
- [Firebase Firestore](https://firebase.google.com/) for storing posts (`blogs` collection)
- Firebase Auth (email/password) for admin access
- Hosted on [Netlify](https://netlify.com), auto-deploys from GitHub

## Adding a new post

Use the admin panel (`ayseyagmur.html`) — no code changes needed. Fields:

| Field | Notes |
|---|---|
| Title | Post title |
| Excerpt | Short teaser shown in the archive/home carousel |
| Date | Format `DD/MM/YYYY` |
| Slug | URL-friendly id, e.g. `eternity-away` |
| Kind | `essay`, `review`, or `poetry` |
| Language | `en` or `tr` |
| Content | Paragraphs separated by a blank line; single line breaks are preserved (useful for poetry) |
| Sign | Optional closing line, shown right-aligned at the bottom |

## Local development

Just open the HTML files in a browser — no server or build step required.
