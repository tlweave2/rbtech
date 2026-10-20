# riverbanktc.com redesign previews

Four design directions for replacing https://www.riverbanktc.com/. All four use the same content and photos, and every claim comes from the current site (see [CLAIMS-AUDIT.md](CLAIMS-AUDIT.md)).

| | Direction | Folder |
|---|---|---|
| A | Civic: calm, public-agency feel | [`previews/a-civic/`](previews/a-civic/index.html) |
| B | Industrial: bold, technical spec-sheet | [`previews/b-industrial/`](previews/b-industrial/index.html) |
| C | Hometown: warm, photo-led, neighborly | [the homepage (`index.html`)](index.htmlindex.html) |
| D | Straight Answers: question-led, based on the uploaded design | [`previews/d-straight-answers/`](previews/d-straight-answers/index.html) |

`index.html` at the root is the hub page that links to all four. `design-source/` holds the original exported design file that D is based on. It is for reference only and was not claim-checked.

## Viewing the previews

**GitHub Pages (recommended for sharing):** go to the repo's Settings → Pages, set Source to "Deploy from a branch", and pick this branch with the `/ (root)` folder. The hub will be at `https://<user>.github.io/rbtech/`, and each preview at `.../previews/<name>/`.

**Locally:** open `index.html` in a browser. No build step is needed.

The content rationale and the open copy issues are in [REDESIGN.md](REDESIGN.md).

## Brand

All previews use the colors and type from the RTC social media flyer:

| Use | Color |
|---|---|
| Navy (text, headings, dark bands) | `#0b2842` |
| Footer navy | `#01284d` |
| Bright blue | `#1586c2` |
| Link and button blue | `#0473b8` |
| Green (labels, accents) | `#4c9225` / `#6ca13e` |
| Muted text | `#516779` |

Headings use Montserrat (800–900), and section labels use widely spaced Montserrat capitals. Body text is Inter. The header shows a text wordmark (RIVERBANK / TECHNOLOGY CENTER). Swap in the real RTC logo file once it is available. The footer has the flyer's blue and green wave band.

## Selected design: C (Hometown)

All contact on preview C goes to **info@riverbanktc.com**: the email link, the contact form, and the "Get project updates" sign-up.

Both forms post to [FormSubmit](https://formsubmit.co), a free service that emails each submission, because GitHub Pages can't process forms itself. Before it goes live:

1. **Activate the address.** The first time either form is submitted from the live site, FormSubmit emails an activation link to info@riverbanktc.com. Someone with access to that inbox has to click it. Submissions are not delivered until then.
2. **Optional: hide the address.** After activation, FormSubmit provides a random alias. Replace `info@riverbanktc.com` in the two form `action` URLs with that alias so the address isn't in the page source.
3. **Subscribers arrive as individual emails** with the subject "RTC website: new email subscriber". To send updates to them, copy them into a mailing tool such as Mailchimp. Or connect the sign-up form directly to that tool later.

After either form is submitted, people see `project/thanks.html`.

## Site structure

| URL | Page |
|---|---|
| `/` | Community Resource Hub, the landing page |
| `/resources/` | The same hub. This is where the town hall QR signs point, so keep it. |
| `/project/` | Full project website (design C), with the contact form and sign-up |
| `/previews/` | The four design directions, not linked from the live site |
