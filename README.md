# adafarkosh.com

Personal portfolio site for Ada Farkosh (Oleksandra Farkosh), motion and 3D artist
based in Cork, Ireland. Hand-written HTML and CSS, with a few lines of JavaScript
for the image lightbox.

## Layout

```
index.html              the work index
projects/               one page per project
style/style.css         the single stylesheet for every page
assets/<project>/       images/ and videos/ for that project
assets/site/            backgrounds, contact tab, icon, docs
```

## Adding a project

1. Put the files in `assets/<project_name>/images/` (and `videos/` if needed).
2. Copy `projects/` nearest existing page, change the content between the
   `PAGE CONTENT` comments, and fix the `current` link in the sidebar.
3. Copy one `<article class="project">` block in `index.html`. The numbering and
   the left/right alternation are done in CSS, so nothing needs renumbering.

## Notes

Project rows number themselves with a CSS counter and alternate sides with
`:nth-of-type`, so reordering the blocks in `index.html` is enough.
Animations are mp4, not gif, and carry `width`/`height` so the page does not
jump while they load.
