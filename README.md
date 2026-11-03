# 💻 The Basics of HTML

Starter files for a coding exercise on common HTML elements and attributes. The four pages
in this repo are plain, unmarked-up text. You will add the HTML structure, then publish the
finished site to GitHub Pages.

These pages are going to look plain in the browser, and that is fine — there is no CSS in
this exercise. The point is to practice using HTML to give content structure and meaning.
Styling comes later in the course.

> [!NOTE]
> `.editorconfig`, `.gitattributes`, `.gitignore`, `.noai`, and the `.github` folder are
> setup files that keep assignments consistent. Leave them alone.

## 📋 Assignment Requirements

The requirements, grading rubric, and due date for this assignment are in
[ASSIGNMENT.md](ASSIGNMENT.md). Read it before you start, and check it again before
you submit. This `README` only covers how to publish and submit your work.

## 🏁 Getting Started

1. On GitHub, click the green **Code** button → **Open with GitHub Desktop**. Pick a folder
   on your computer and click **Clone**. (Already have GitHub Desktop open? Use
   **File** → **Clone Repository** instead.)
2. In GitHub Desktop, create your assignment branch: **Current Branch** → **New Branch**.
   Name it something like `assignment` or `your-name`.
3. Click **Open in \<editor\>** to open the folder in your code editor and start working.

> [!IMPORTANT]
> Open the whole project **folder** in your editor, not a single HTML file on its own.
> This exercise uses images and links between files, and your editor can only resolve
> those paths if it can see every file in the project.

## 📂 Where Your Files Go

Every file you need is already in this repo. The four pages you are marking up are in the
**root folder** — the same folder as this README. Edit them where they are.

```
index.html
common.html
images.html
links.html
logo.png
resources/
  cat.jpg
  otherpage.html
```

Do not rename or move these files. You link between them by name, and `index.html` in
particular has to keep its name and stay in the root folder — GitHub Pages publishes from
the root and serves `index.html` as your home page. Rename it and your site will 404.

## 🤖 AI Policy

Work on this assignment must be your own. Do not use AI coding assistants — including
GitHub Copilot, Cursor, ChatGPT, Claude, or JetBrains AI Assistant — to generate,
complete, or rewrite your code.

You should be able to explain any line of your submission. You may be asked to do so.

This repo includes a `.noai` file, which disables JetBrains AI Assistant for the project
in IDEs like WebStorm. Leave it in place. It is a reminder of the policy above, not a
substitute for it — following the policy is still your responsibility.

## 🚀 Publishing to GitHub Pages

Your work has to be live on the web before you can submit it.

1. In **GitHub Desktop**, commit your work to your assignment branch, then push it.
   - Enter a summary in the bottom-left box and click **Commit to \<branch\>**.
   - Click **Push origin** at the top.
2. On GitHub, open this repo and go to **Settings** → **Pages**. Set **Source** to *Deploy from a branch*, pick your assignment branch with folder `/ (root)`, and click **Save**. The first deploy takes a minute or two.
3. Reload the Pages settings screen and open the live URL it gives you:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```
   Confirm the page loads correctly — the right content, no missing images, no broken links.

**🛠️ Troubleshooting the deploy**

- **404 page:** make sure `index.html` is still in the root of the branch you selected, still lowercase, and that you committed it.
- **Old version showing:** Pages caches aggressively. Wait a minute, then hard refresh (<kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd>).
- **Nothing deployed:** check the **Actions** tab for a failed `pages build and deployment` run.
- **Images or links work locally but break on Pages:** the live site is case-sensitive even
  if your computer is not. `Logo.png` and `logo.png` are the same file on macOS and
  Windows, but different files on GitHub Pages. Check that your `src` and `href` values
  match the real filenames exactly.
- **An image or page is missing from the live site:** confirm you actually committed it.
  In GitHub Desktop, a file that never appeared in the **Changes** list was never pushed.

**🛠️ Troubleshooting your HTML**

If a page is not rendering the way you expect, check these first:

- Did you save the file?
- Is your content inside the `body` element?
- Is every opening tag matched with a closing tag, in the right order?
- Are your attribute values wrapped in quotation marks?
- Is the file name — and its extension — spelled exactly right in your `src` or `href`?
- Is the file actually in the folder your path says it is in?

To a browser, `cat.jpg`, `Cat.jpg`, `cat.jpeg`, `resources/cat.jpg`, and `resource/cat.jpg`
are five different things. The browser does not know what you meant; it follows exactly
what you typed. If you want a second opinion on your markup, paste it into the
[W3C validator](https://validator.w3.org/#validate_by_input).

## 📬 Submitting the Assignment

Submission has two parts: publish the site, then submit a pull request URL in Canvas.

1. **Publish to GitHub Pages** using the steps above. Do this first.
2. **Open a pull request into `main`.**
   - In **GitHub Desktop**, with your assignment branch selected, choose **Branch** → **Create Pull Request**. The pull request form opens in your browser.
   - Confirm **base** is `main` and **compare** is your assignment branch.
   - Title it with the assignment name.
   - Paste your live GitHub Pages URL into the description.
   - Click **Create pull request**.
3. **Copy the pull request URL** from your browser's address bar and submit it in Canvas under the matching assignment.


> [!CAUTION]
> Late or missing submissions are graded on what is in the pull request at the deadline, so push your final commits before you submit.
