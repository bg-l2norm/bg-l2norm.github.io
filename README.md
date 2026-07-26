# bg-l2norm.github.io

A minimal Jekyll site with three primary pages: Home, Blog, and Notes.

## Home events

Edit `_data/events.yml`. Each event supports:

```yaml
- id: unique-event-id
  title: "Event title"
  date: "YYYY-MM-DD"
  summary: "One-line summary"
  body: |
    Event details in Markdown.
  url: "https://example.com"
  link_label: "Open link"
```

The Home page renders events as an inbox-style list. Selecting an event expands it
for focused reading. The same events also appear in the right-hand site index.

## Blog posts

Create `_posts/YYYY-MM-DD-title.md`:

```yaml
---
title: "Post title"
categories: []
---

Post content.
```

## Notes

Create `_notes/title.md`:

```yaml
---
title: "Note title"
summary: "One-line summary"
---

Note content.
```

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000`.

## Header banner

The Rosenbrock shooting-star banner is shown globally on every page. Its full-width off-black container has a bounded responsive height to prevent layout changes between refreshes.
