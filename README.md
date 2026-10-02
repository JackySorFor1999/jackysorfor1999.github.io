# My first GitHub Pages website

This is a starter personal website made with plain HTML and CSS. You can edit it without installing a framework or a package manager.

## How it works

- `index.html` contains the page content and structure: headings, paragraphs, sections, and links. GitHub Pages serves this file as your homepage.
- `styles.css` controls the appearance: colors, fonts, spacing, and layout. The `<link>` inside `index.html` connects the stylesheet to the page.
- `README.md` is this guide, shown on your repository's GitHub page.
- `.gitignore` tells Git which local files to leave out. It ignores `.DS_Store`, a macOS Finder settings file, in every folder.

Git stores the history of your files. GitHub hosts your repository. GitHub Pages publishes the website files so people can view them in a browser.

## 1. Preview your website

Open the repository folder in Finder and double-click `index.html` to open it in a browser. If it opens in an editor, right-click it and choose **Open With** → your browser.

After editing a file, save it and refresh the browser to see your changes. This starter works directly from the file; no server is required.

## 2. Make it yours

Open `index.html` in your editor. For example, change:

```html
<h1 id="intro-heading">Hello, I'm Jacky.<br>This is my website.</h1>
```

to:

```html
<h1 id="intro-heading">Hi, I'm Jacky.<br>Welcome to my website.</h1>
```

`<h1>` is the main heading, and `<br>` starts a new line. The text inside `<p>...</p>` is a paragraph. A link looks like `<a href="https://example.com">Link text</a>`.

Next, replace the About me paragraph and update the browser-tab title inside `<title>...</title>`. To add a project, copy the entire `<article class="project-card">...</article>` block and change its title, description, and link.

Open `styles.css` to change the design. Start with `--accent: #0069b4;` near the top: this controls the link and keyboard-focus color. The `.button` and `.site-header` rules use `linear-gradient(...)` to create Aqua's glossy blue and silver surfaces. Save and refresh to see the result.

The minimal Aqua styling takes inspiration from [Apple's January 5, 2004 homepage](https://web.archive.org/web/20040105094327/http://www.apple.com/): a white background, silver tabs, fine borders, and generous whitespace. All effects are made with CSS; no external images, fonts, or JavaScript are needed.

## 3. Upload your files to GitHub

In a terminal opened in this repository folder, run:

```sh
git add index.html styles.css README.md
git commit -m "Add my first website"
git push origin main
```

- `git add` selects the files to include in your next saved version.
- `git commit` records that version locally with a description.
- `git push` uploads your commits to GitHub. Authenticate if GitHub asks you to sign in.

## 4. Enable GitHub Pages

1. Open [your repository](https://github.com/JackySorFor1999/jackysorfor1999.github.io).
2. Go to **Settings** → **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch** as the source.
4. Choose the **main** branch and **/(root)** folder, then click **Save**.
5. Wait a few minutes for deployment. The repository's **Actions** tab shows its progress, and **Settings** → **Pages** shows the published URL.
6. Visit **https://jackysorfor1999.github.io/**.

The repository name follows GitHub's `username.github.io` convention, so this is your personal site's address. Keep `index.html` at the top level of the repository, alongside this README.

If you see a 404, check that `index.html` has been pushed to `main`, that Pages uses `main` and `/(root)`, and that the deployment has finished. GitHub Free requires a public repository for Pages; private repository support depends on your plan.

## 5. Keep improving it

For every update: edit → save → preview → commit → push. Once Pages is enabled, pushing to `main` triggers publication of the new version.

If the live website still looks old after pushing:

1. Open the repository's **Actions** tab and wait for **pages build and deployment** to finish successfully for your latest commit. Uploading the files and publishing the site are separate steps.
2. Open the website in a private browser window to check for a cached copy. In Chrome on a Mac, **Command + Shift + R** reloads the page without using its cached files; in Safari, use **Option + Command + R**.
3. If the deployment succeeded but the site is still old, wait a few minutes and try again. GitHub Pages also caches published files for a short time.

Adding a file to `.gitignore` does not remove a copy Git already tracks. For an accidentally tracked `.DS_Store`, `git rm --cached .DS_Store` removes it from Git while keeping it on your Mac; commit and push that removal along with `.gitignore`.

JavaScript is optional. You can add it later if you need interactive behavior, such as a theme switcher. HTML and CSS are enough for this personal homepage.

Remember that published website files are public. Keep passwords, API keys, and private information out of them.

More help: [GitHub Pages documentation](https://docs.github.com/en/pages).
