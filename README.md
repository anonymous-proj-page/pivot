# PIVOT — anonymous project page

Self-contained static project page for double-blind review. **No external resources, no external
links, no identifying information.**

## Structure

```
index.html              # the page (real anonymized text; media slots are placeholders)
css/style.css           # local stylesheet, system fonts only
assets/
  videos/               # drop video files here (see assets/PLACEHOLDERS.md)
  images/               # drop figure images here
  PLACEHOLDERS.md       # exact expected filenames + specs
.nojekyll               # serve files as-is on GitHub Pages
```

## Adding media

Media is intentionally left empty. For each slot in `index.html`, uncomment the adjacent
`<video>` / `<img>` tag and remove the placeholder `<div>`. See `assets/PLACEHOLDERS.md` for the
expected file paths and specs.

## Local preview

```
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy (GitHub Pages)

Push these files to the repository root and enable GitHub Pages from the root of the default
branch. The page is served as-is (`.nojekyll`).

## Anonymity notes

- The page itself makes **zero external network requests** and contains no author/affiliation
  information or outbound links.
- Git is configured with an anonymous local identity; commits carry no real name/email.
- **Caveat:** the hosting GitHub account / repository URL can still deanonymize you. For a truly
  blind submission, host under a throwaway account or an anonymizing mirror.
