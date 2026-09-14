# Hansol Suh's website

Static personal website: `index.html`, `projects.html`, `publications.html`, and
`talks.html`, with shared styles in `main.css`.

Preview locally with `python3 -m http.server 8000`, then open
`http://localhost:8000`.

The CV source is `assets/hansol-suh-cv.tex`. Rebuild with a TeX Live installation:

```sh
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=/tmp assets/hansol-suh-cv.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=/tmp assets/hansol-suh-cv.tex
cp /tmp/hansol-suh-cv.pdf assets/hansol-suh-cv.pdf
```

Keep publication titles, author order, and statuses consistent between the HTML
pages and the CV source. Navigation is shared by convention; update all four pages
when adding a page.
