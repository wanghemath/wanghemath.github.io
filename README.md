
# He Wang — Personal Academic Website

This repository contains the source files for my personal academic website:

**Website:** [https://wanghemath.github.io/](https://wanghemath.github.io/)

**GitHub Repository:** [https://github.com/wanghemath/wanghemath.github.io](https://github.com/wanghemath/wanghemath.github.io)

The website is built with **Quarto** and hosted using **GitHub Pages**.

---

## About the Website

This site serves as my professional and academic homepage. It includes information about my teaching, research interests, academic programs, student projects, and educational resources.

The main goals of the website are to:

* present my academic profile and professional background;
* share teaching materials and course-related resources;
* highlight research interests and ongoing projects;
* provide information for students, collaborators, and prospective applicants;
* organize links to books, lecture notes, labs, and GitHub-hosted teaching materials.

---

## Main Sections

The website may include pages such as:

* **Home** — overview, profile, contact information, and highlights.
* **Teaching** — courses taught, teaching philosophy, course links, and educational resources.
* **Research** — research interests, selected projects, and publications.
* **Programs** — information about graduate programs and curriculum initiatives.
* **Projects** — student projects, applied mathematics projects, data science projects, and AI-related work.
* **Resources** — links to lecture notes, books, labs, GitHub repositories, and interactive materials.

---

## Technology Used

This website is created using:

* [Quarto](https://quarto.org/)
* Markdown / QMD files
* HTML / CSS
* GitHub Pages
* Git and GitHub

Quarto allows the site to combine text, mathematics, code, figures, links, and interactive content in a clean academic format.

---

## Repository Structure

A typical structure of this repository is:

```text
.
├── _quarto.yml          # Quarto website configuration
├── index.qmd            # Home page
├── teaching.qmd         # Teaching page
├── research.qmd         # Research page
├── programs.qmd         # Program information page
├── projects.qmd         # Projects page
├── styles.css           # Custom CSS styling
├── docs/                # Rendered website files for GitHub Pages
├── images/              # Images, profile photos, and diagrams
└── README.md            # Repository description
```

The exact file names may change as the website develops.

---

## Local Editing Workflow

To edit the website locally:

1. Open the repository folder on your computer.

2. Edit the `.qmd`, `.yml`, `.css`, or image files.

3. Render the website:

```bash
quarto render
```

4. Preview the website locally:

```bash
quarto preview
```

5. Add, commit, and push changes to GitHub:

```bash
git add .
git commit -m "Update website"
git push origin main
```

---

## GitHub Pages Deployment

This website is deployed through GitHub Pages.

For this repository, the GitHub Pages settings should usually be:

```text
Source: Deploy from a branch
Branch: main
Folder: /docs
```

This assumes that `_quarto.yml` contains:

```yaml
project:
  type: website
  output-dir: docs
```

After each push to the `main` branch, GitHub Pages rebuilds and updates the public website automatically.

The website is available at:

https://wanghemath.github.io/

---

## Common Update Commands

For routine updates, use:

```bash
quarto render
git add .
git commit -m "Update Quarto website"
git push origin main
```

If GitHub has remote changes and the push is rejected, first pull and rebase:

```bash
git pull --rebase origin main
git push origin main
```

If the goal is to replace the GitHub version completely with the local version, use force push carefully:

```bash
git push --force origin main
```

Use force push only when you are sure the local version is the correct version to keep.

---

## Notes for Maintenance

Before pushing updates, it is helpful to check:

```bash
git status
```

To confirm the GitHub remote:

```bash
git remote -v
```

To render the Quarto website:

```bash
quarto render
```

To check that the rendered website files are generated correctly, open the `docs/` folder and confirm that `index.html` and related files exist.

---

## Related Links

* Personal Website: https://wanghemath.github.io/
* GitHub Profile: https://github.com/wanghemath
* Quarto Documentation: https://quarto.org/docs/websites/
* GitHub Pages Documentation: https://docs.github.com/en/pages

---

## License

Unless otherwise stated, the materials in this repository are intended for educational and academic use.

Please contact the author before reusing substantial portions of the website content, course materials, or original diagrams.

---

## Author

**He Wang**
Department of Mathematics
Northeastern University

Website: https://wanghemath.github.io/
