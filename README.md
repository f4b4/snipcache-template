# SnipCache

A collection of know-how snippets: recipes, scripts, SQL, keyboard shortcuts
and whatever else is worth keeping. Every push to this repository publishes it
as a searchable website on GitHub Pages. This `README.md` is the site's home
page, so make it your own.

## Adding snippets

- Folders become groups in the sidebar, nested as deep as you like.
- Markdown files (`.md`) are rendered as pages. The page title is the
  frontmatter `title`, else the first `# Heading`, else the file name.
- Every other text file (`.sql`, `.ps1`, `.sh`, `.bat`, …) becomes a page with
  the whole file in one highlighted code block.
- A `README.md` inside a folder is that folder's index page.
- Every page has buttons to copy the whole file and to open the raw file.
- Files and folders starting with a dot are ignored.

## Setting up your own copy

1. Create a repository from this template ("Use this template").
2. In the new repository, open Settings → Pages and set Source to
   "GitHub Actions".
3. Run the "Deploy SnipCache" workflow once (Actions → Deploy SnipCache →
   Run workflow). After that, every push to `main` updates the site.
4. Optionally set `site_title` and `editor_url` in
   `.github/workflows/deploy.yml`.

The site appears at `https://<owner>.github.io/<repository>/`. The full guide
is in the [SnipCache repository](https://github.com/f4b4/snipcache/blob/main/doc/content-repo-guide.md).
