# whiskers & ferments - Hugo Site

This is a Hugo-based version of whiskers and ferments. All content is now in markdown files, making it easy to write and maintain.

## How to Use

### Run the Development Server

```bash
hugo server -D
```

This will start a local server at `http://localhost:1313/` and watch for changes.

### 3. Build for Production

```bash
hugo
```

This generates static HTML files in the `public/` directory.

## Site Structure

- `config.toml` - Site configuration
- `content/` - Markdown content files
  - `_index.md` - Home page
  - `about.md` - About page
  - `blog/` - Blog posts
    - `_index.md` - Blog list page
    - `*.md` - Individual blog posts
- `layouts/` - HTML templates
  - `_default/baseof.html` - Base template
  - `_default/list.html` - List pages (blog index)
  - `_default/single.html` - Single pages (about, blog posts)
  - `index.html` - Home page template
- `static/styles.css` - CSS styles (same as original)

## Adding New Blog Posts

1. Create a new markdown file in `content/blog/` (e.g., `content/blog/my-new-post.md`)
2. Add frontmatter with title and date:

```markdown
---
title: "My New Post"
date: 2026-11-14
---

Your content here...
```

3. Write your content in markdown

## Hugo Features Used

- **Markdown content** - Write in easy-to-read markdown
- **Templating** - Consistent layout across all pages
- **Taxonomies** - Blog posts are automatically organized
- **Shortcodes** - Available for special content (optional)
