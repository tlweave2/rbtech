# riverbanktc.com redesign previews

Four design directions for replacing https://www.riverbanktc.com/. All four use the same content and photos, and every claim comes from the current site (see [CLAIMS-AUDIT.md](CLAIMS-AUDIT.md)).

| | Direction | Folder |
|---|---|---|
| A | Civic: calm, public-agency feel | [`previews/a-civic/`](previews/a-civic/index.html) |
| B | Industrial: bold, technical spec-sheet | [`previews/b-industrial/`](previews/b-industrial/index.html) |
| C | Hometown: warm, photo-led, neighborly | [`previews/c-hometown/`](previews/c-hometown/index.html) |
| D | Straight Answers: question-led, based on the uploaded design | [`previews/d-straight-answers/`](previews/d-straight-answers/index.html) |

`index.html` at the root is the hub page that links to all four. `design-source/` holds the original exported design file that D is based on. It is for reference only and was not claim-checked.

## Viewing the previews

**GitHub Pages (recommended for sharing):** go to the repo's Settings → Pages, set Source to "Deploy from a branch", and pick this branch with the `/ (root)` folder. The hub will be at `https://<user>.github.io/rbtech/`, and each preview at `.../previews/<name>/`.

**Locally:** open `index.html` in a browser. No build step is needed.

The content rationale and the open copy issues are in [REDESIGN.md](REDESIGN.md).
