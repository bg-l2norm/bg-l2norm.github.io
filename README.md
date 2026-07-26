# Raw academic GitHub Pages site

A deliberately plain personal site for blog posts, notes, achievements, and
occasional images. It uses Jekyll, which GitHub Pages can build directly.

## 1. Create the repository

Create a public repository named:

```text
bg-l2norm.github.io
```

Copy these files into it. The GitHub username and email are already configured;
edit the display name and description later if desired.

## 2. Enable GitHub Pages

In the repository:

1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select `main` and `/ (root)`.

The site will be published at `https://bg-l2norm.github.io`.

## 3. Enable comments with giscus

1. Keep the repository public.
2. Enable **Settings → General → Features → Discussions**.
3. Install the giscus GitHub App for the repository.
4. Open `https://giscus.app`, enter the repository, choose the **pathname**
   mapping, and choose a discussion category.
5. Copy the generated `repo`, `repo-id`, `category`, and `category-id` values
   into `_config.yml`.

Visitors need a GitHub account to comment. Comments are stored as GitHub
Discussions and can be moderated there.

## 4. Write

### Blog post

Create `_posts/YYYY-MM-DD-title.md`:

```yaml
---
title: "Post title"
categories: [math, reading]
---

Post body in Markdown.
```

Comments are on by default. Disable them on a particular post with:

```yaml
comments: false
```

### Note

Create `_notes/name.md`:

```yaml
---
title: "Note title"
summary: "One-line description."
---

Living note in Markdown.
```

## 5. Preview locally

With Ruby and Bundler installed:

```bash
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000`.
