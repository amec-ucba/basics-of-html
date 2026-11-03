# 💻 Assignment Boilerplate

A starting point for assignment and exercise repos. It includes submission instructions, editor and Git configuration, and a pull request template so every assignment works the same way.

> [!NOTE]
> `.editorconfig`, `.gitattributes`, `.gitignore`, `.noai`, and the `.github` folder are
> setup files that keep assignments consistent. Leave them alone.

## 📋 Assignment Requirements

The requirements, grading criteria, and due date for this assignment are in
[ASSIGNMENT.md](ASSIGNMENT.md). Read it before you start, and check it again before
you submit. This `README` only covers how to publish and submit your work.

## 🏁 Getting Started

1. On GitHub, click the green **Code** button → **Open with GitHub Desktop**. Pick a folder
   on your computer and click **Clone**. (Already have GitHub Desktop open? Use
   **File** → **Clone Repository** instead.)
2. In GitHub Desktop, create your assignment branch: **Current Branch** → **New Branch**.
   Name it something like `assignment` or `your-name`.
3. Click **Open in \<editor\>** to open the folder in your code editor and start working.

## 📂 Where Your Files Go

Create your files in the **root folder** of this repo — the same folder as this README.
GitHub Pages publishes from the root, so `index.html` has to live there or your site will 404. Group your assets into subfolders:

```
index.html
css/style.css
js/script.js
images/photo.jpg
```

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
   Confirm the page loads correctly — the right content, no missing images, no broken styles.

**🛠️ Troubleshooting**

- **404 page:** make sure an `index.html` exists in the root of the branch you selected, and that the filename is lowercase.
- **Old version showing:** Pages caches aggressively. Wait a minute, then hard refresh (<kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd>).
- **Nothing deployed:** check the **Actions** tab for a failed `pages build and deployment` run.

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
