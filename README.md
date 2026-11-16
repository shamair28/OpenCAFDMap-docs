# Open CAFD Map documentation

The documentation site for [Open CAFD Map](https://github.com/shamair28/OpenCAFDMap) and OpenLauncher:
**https://shamair28.github.io/OpenCAFDMap-docs/**

Built with [Zola](https://www.getzola.org/) and the [book](https://github.com/getzola/book) theme, starting from
the [book-template](https://github.com/sakkke/book-template) layout.

## Editing
- Pages are Markdown files in `content/`. Each folder is a chapter (`_index.md`), and the files in it are its pages,
  ordered by `weight`.
- Pages with images are folders (`page-name/index.md` with the images next to it).
- Link to other pages with `@/chapter/page.md`, so the build checks the link.

```
git clone --recurse-submodules https://github.com/shamair28/OpenCAFDMap-docs
zola serve        # preview at http://127.0.0.1:1111
zola check        # build + check links
```

Every push to `main` builds the site and publishes it to the `gh-pages` branch (`.github/workflows/zola.yml`).
