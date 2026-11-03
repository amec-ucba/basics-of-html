# 📄 The Basics of HTML

**Course:** AMEC ____
**Due:** ____ at ____
**Points:** 15

## 🎯 Overview

This repo contains four unfinished web pages. Right now they are just plain text — no
doctype, no tags, no structure. Your job is to mark that text up with the correct HTML
elements and attributes, then publish the finished site to GitHub Pages.

You have already seen the basic structure of an HTML page: the doctype, `html`, `head`,
`title`, and `body`. This assignment gives you more practice with that structure while
introducing most of the common elements and attributes you will use for the rest of the
course.

Do not worry that these pages will not look impressive. **They are supposed to look
plain.** You are not writing any CSS yet. Right now the goal is to use HTML to give
content *structure and meaning*. Colors, fonts, spacing, and layout come later.

The one rule that matters most: **choose an element because of what the content means, not
because of how the element looks by default.** If something is a heading, use a heading
element. If it is a list, use a list. You can make anything look like anything with CSS
later, so never pick a tag for its appearance.

## 📋 Requirements

### Every page

- [ ] Has a complete HTML document structure — `<!DOCTYPE html>`, `html`, `head`, `body`
- [ ] Has a meaningful, page-specific `<title>` that describes that page
- [ ] Has **all** visible content inside the `body` element
- [ ] Uses one `h1` for the main topic of the page
- [ ] Uses `h2` for major sections and `h3` for subsections inside an `h2` section
- [ ] Wraps every chunk of body text in a `p` element
- [ ] Opens and closes every tag correctly, and quotes every attribute value
- [ ] Opens in a browser with no leftover raw text sitting outside an element

### `index.html` — structure and headings

This is the first page of the exercise and the one GitHub Pages serves at your published
URL, so it has to keep its filename.

- [ ] Stays named `index.html`, in the root folder, all lowercase
- [ ] "The Basics of HTML" is the `h1`
- [ ] "What is HTML?", "HTML Document Structure", and "HTML Syntax" are `h2` elements
- [ ] "Elements", "Tags", and "Attributes" are `h3` elements, because they are subsections
      *inside* the "HTML Syntax" section
- [ ] The four items `!DOCTYPE`, `html`, `head`, and `body` are marked up as an unordered
      list with `li` elements
- [ ] Headings are chosen by importance and structure, not by how big they look

### `common.html` — common building block elements

- [ ] Each of the eight topics ("Headings", "Paragraphs", "Lists", and so on) is an `h2`
- [ ] The numbered list is an `ol`; the bulleted list is a `ul`; both use `li` elements
- [ ] `UCBA` uses `abbr` with a `title` attribute spelling out the full college name, so
      the full name appears on hover
- [ ] The UC Blue Ash address uses `br` to break the lines — not empty paragraphs, and not
      to create blank space
- [ ] The spaced-out "So I can have text like this" block uses `pre`, so the whitespace is
      preserved exactly
- [ ] `strong`, `u`, `mark`, and `sup` are each used on the text that the page describes
      (including the `st` in "October 31st" as a `sup`)

### `images.html` — images, paths, and captions

- [ ] `logo.png` is added where the comment says, using an `img` element with **both**
      `src` and `alt`
- [ ] The `alt` text actually describes the image — not `"logo.png"` or `"image"`
- [ ] The list of file types (`.jpg`, `.png`, `.gif`, …) is marked up as a list
- [ ] A `figure` is added where the second comment says, containing `cat.jpg` from the
      `resources` subfolder with a correct relative path (`resources/cat.jpg`)
- [ ] That `figure` includes a `figcaption` reading **Ivan**, below the image
- [ ] Both images display in the browser — no broken image icons

### `links.html` — hyperlinks

- [ ] The absolute link uses a full URL starting with `https://` to the University of
      Cincinnati website
- [ ] "HTML Basics" is a relative link to `index.html`
- [ ] The subdirectory link is a relative link to `resources/otherpage.html`
- [ ] The email link uses `href="mailto:..."` with a real email address
- [ ] The `target="_blank"` example is left intact and still works
- [ ] Every link is clickable and lands on the right destination when tested in a real
      browser (not the editor preview, which cannot load external sites)

### Publishing and submitting

- [ ] Work is committed and pushed to your assignment branch
- [ ] The site is live on GitHub Pages and the URL loads `index.html`
- [ ] A pull request into `main` is open with the live Pages URL in the description
- [ ] The pull request URL is submitted in Canvas

## 🖼️ Example Output

Your finished site should open on `index.html`, "The Basics of HTML". Each of the four
pages should read as a clean outline: one main heading, clear section headings, real
paragraphs, real lists, and two images that load on `images.html`.

Everything will be black Times New Roman text on a white background. That is the correct
result. If your page looks plain but the *structure* is right, you are done.

<!-- Instructor: add a screenshot here if you want one. -->
<!-- ![Example output](images/example.png) -->

## 📂 Starter Files

| File / Folder | Purpose | You edit it? |
| --- | --- | --- |
| `index.html` | Page 1 — document structure and headings; also the page GitHub Pages serves | ✅ Yes |
| `common.html` | Page 2 — common text elements and lists | ✅ Yes |
| `images.html` | Page 3 — images, file paths, figures | ✅ Yes |
| `links.html` | Page 4 — absolute, relative, and email links | ✅ Yes |
| `logo.png` | Image used on `images.html` | No — just link to it |
| `resources/cat.jpg` | Image used in the `figure` on `images.html` | No — just link to it |
| `resources/otherpage.html` | Already-finished page, the target of a relative link | No — leave as is |

> [!WARNING]
> File and folder names are exact. To a browser, `cat.jpg`, `Cat.jpg`, `cat.jpeg`, and
> `resource/cat.jpg` are four different things, and three of them are broken. The browser
> does not know what you meant — it only follows what you typed.

## 🧮 Grading

| Criteria | What earns full credit | Points |
| --- | --- | --- |
| **Document structure** | All four pages have a correct doctype, `html`, `head`, and `body`; all visible content is inside `body`; each page has its own meaningful `title`. | 2 |
| **Headings and paragraphs** | `h1`/`h2`/`h3` reflect the real outline of each page rather than visual size; body text is in `p` elements. | 2 |
| **`common.html` elements** | `ol`, `ul`, `li`, `abbr` with `title`, `br`, `pre`, `strong`, `u`, `mark`, and `sup` are all present and used on the content they describe. | 4 |
| **Images and paths** | `logo.png` and `resources/cat.jpg` both display; `src` paths are correct; `alt` text is descriptive; `figure` wraps the cat image with a `figcaption` reading "Ivan". | 3 |
| **Links** | Absolute, relative, subdirectory, and `mailto:` links are all present, correctly formed, and go to the right place. | 3 |
| **Published and submitted** | GitHub Pages site is live and loads correctly; pull request into `main` is open with the live URL in the description; PR URL submitted in Canvas. | 1 |
| **Total** |  | **15** |

### 🔻 Deductions

Taken out of the totals above, capped at 5 points.

| Issue | Deduction |
| --- | --- |
| Broken image or broken link on the live site | −1 each |
| Raw text left outside of any element | −1 each |
| Unclosed tag or unquoted attribute value | −1 each |
| `title` left as "Document" or copied between pages | −1 each page |
| Starter file deleted, renamed, or left unedited | −2 each |

## ✅ Before You Submit

Walk your **live Pages site** — not your local files — and check:

- [ ] `index.html` loads at the Pages URL, and all four links work from it
- [ ] Every page has a title in the browser tab that describes that page
- [ ] No broken image icons anywhere
- [ ] Every link goes somewhere real, including the email and subdirectory links
- [ ] "View Page Source" in the browser shows a doctype at the top of every page
- [ ] You can explain why you chose each element you used

## 📚 Resources

- [MDN — HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [MDN — HTML basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
- [MDN — `<figure>` and `<figcaption>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
- [MDN — Creating hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)
- [W3C Markup Validation Service](https://validator.w3.org/#validate_by_input) — paste your
  HTML in to catch unclosed tags
- Canvas: the screencast videos for this assignment, in order

## 🆘 Getting Help

- Post in the Canvas discussion board — if you are stuck, someone else probably is too
- Bring the exact error or the page that is not working; "it doesn't work" is hard to debug

Coding is detail-oriented, and small mistakes are completely normal while you are
learning. Slow down, read the path you typed, and check it character by character.

---

The AI policy and submission instructions are in the [README](README.md).
