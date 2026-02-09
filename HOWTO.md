# How to Update Your Personal Website

Your site lives at: https://drjackxiaoyuchen.github.io
Repo: https://github.com/Drjackxiaoyuchen/drjackxiaoyuchen.github.io

## Quick Start: The Edit-Commit-Push Cycle

Every change follows the same pattern:

```bash
cd ~/drjackxiaoyuchen.github.io

# 1. Edit files (see sections below for what to edit)
# 2. Preview locally (optional)
export PATH="/opt/homebrew/opt/ruby/bin:/opt/homebrew/lib/ruby/gems/3.4.0/bin:$PATH"
bundle exec jekyll serve --port 8080
# Open http://localhost:8080

# 3. Push to make it live
git add -A
git commit -m "Describe what you changed"
git push
# Wait ~2 minutes for GitHub Actions to deploy
```

---

## Common Tasks

### Update your bio / about page
**File:** `_pages/about.md`

The top section (between `---` markers) is YAML config. Below it is your bio in Markdown.

```markdown
---
subtitle: Your Title, <a href='https://company.com'>Company</a>
profile:
  image: prof_pic.png    # put new image in assets/img/
  more_info: >
    <p>Your Company</p>
    <p>Your City</p>
---

Your bio text goes here. Use [links](https://example.com) and **bold**.
```

### Change your profile picture
1. Put your new photo in `assets/img/` (name it `prof_pic.png` or `prof_pic.jpg`)
2. Update the `image:` line in `_pages/about.md` to match the filename

### Update your CV
**Two files to update** (they show the same data in different formats):

- `_data/cv.yml` — Used by the interactive CV page (RenderCV format)
- `assets/json/resume.json` — JSON Resume format (alternative)

In `_data/cv.yml`, the structure is:
```yaml
cv:
  sections:
    Experience:
      - company: Company Name
        position: Your Title
        location: City, State
        start_date: 2026-01
        end_date: present
        summary: What you did.
    Education:
      - institution: University Name
        area: Your Field
        studyType: Ph.D.
        start_date: 2017
        end_date: 2021
```

### Replace your CV PDF
Put your new PDF at: `assets/pdf/Jack_xiaoyu_chen_CV.pdf`
(or change the path in `_data/socials.yml` and `_pages/cv.md`)

### Add a publication
**File:** `_bibliography/papers.bib`

Add a new BibTeX entry:
```bibtex
@article{yourkey2026,
  abbr      = {Journal},
  title     = {Your Paper Title},
  author    = {Chen, J.X. and Coauthor, A.},
  journal   = {Journal Name},
  year      = {2026},
  doi       = {10.xxxx/xxxxx},
  selected  = {true},
  bibtex_show = {true}
}
```
- `selected = {true}` — shows it on the homepage under "selected publications"
- `abbr` — the badge shown next to the paper
- `bibtex_show = {true}` — shows a "Bib" button to view the raw citation

### Add a news/announcement item
**Folder:** `_news/`

Create a new file like `_news/announcement_6.md`:
```markdown
---
layout: post
date: 2026-03-15 10:00:00-0500
inline: true
related_posts: false
---

Your announcement text with **bold** and [links](https://example.com).
```

### Add a blog post
**Folder:** `_posts/`

Create a file named `YYYY-MM-DD-your-title.md`:
```markdown
---
layout: post
title: Your Post Title
date: 2026-03-15 12:00:00
description: A short description.
tags: fiction essays science
categories:
---

Your post content in Markdown.
```

### Add a book to your reading list
**Folder:** `_books/`

Create a file like `_books/book_name.md`:
```markdown
---
layout: book-review
title: Book Title
author: Author Name
olid: OL12345M
categories: science-fiction novels
date: 2026-01-15
started: 2026-01-01
finished: 2026-01-15
released: 2020
stars: 4
status: Finished
---

Your review text.
```
- `olid` — Open Library ID (for auto-fetching cover art). Find it at https://openlibrary.org
- `status` — `Finished`, `Reading`, or `Want to Read`

### Update social links
**File:** `_data/socials.yml`

```yaml
email: your@email.com
scholar_userid: your_google_scholar_id
linkedin_username: your-linkedin
github_username: your-github
cv_pdf: /assets/pdf/Your_CV.pdf
```

### Change site title or description
**File:** `_config.yml`

```yaml
first_name: Jack Xiaoyu
last_name: Chen
description: >
  Your site description for SEO.
keywords: your, keywords, here
```

Note: Changes to `_config.yml` require restarting the local server.

### Add/remove navigation pages
Each page in `_pages/` has a header with `nav: true/false` and `nav_order: N`.
- `nav: true` — shows in the top navigation bar
- `nav_order: 1` — controls the order (lower = further left)

---

## File Structure Cheat Sheet

```
_pages/about.md          → Homepage (/)
_pages/publications.md   → Publications page
_pages/cv.md             → CV page
_pages/books.md          → Reading list
_pages/blog.md           → Writing/blog page

_bibliography/papers.bib → Your publications (BibTeX)
_data/cv.yml             → CV data
_data/socials.yml        → Social links & email
assets/json/resume.json  → CV data (JSON format)

_news/                   → News announcements
_posts/                  → Blog posts
_books/                  → Book reviews

assets/img/prof_pic.png  → Profile photo
assets/pdf/              → CV and other PDFs

_config.yml              → Site-wide settings (name, URL, etc.)
```

---

## Tips

- **Preview before pushing:** Always run `bundle exec jekyll serve --port 8080` locally to check your changes before pushing
- **Markdown basics:** `**bold**`, `*italic*`, `[link text](url)`, `# Heading`
- **Images in posts:** Put images in `assets/img/` and reference them as `![alt text](/assets/img/filename.jpg)`
- **Deploy takes ~2 min:** After `git push`, wait for the GitHub Actions "Deploy site" workflow to finish
- **Config changes need restart:** If you edit `_config.yml`, you need to restart the local Jekyll server
