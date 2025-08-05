# How to Update the Website

This is a step-by-step guide for updating the Quarto website hosted on GitHub Pages. Follow these instructions after editing any `.qmd` file.

---

## 1. Render the Website

In the terminal:

quarto render


This converts `.qmd` files into HTML in the `_site/` folder.

---

## 2. (Optional) Preview the Website Locally

To view the site before uploading:

quarto preview


Use Ctrl+C to stop previewing.

---

## 3. Stage the Changes

In the terminal:

git add .


---

## 4. Commit the Changes

git commit -m "Updates"


Example: git commit -m "Update index page content"


---

## 5. Push to GitHub

git push


---

## 6. Check the Live Site

Visit: [https://www.paulfordethics.com](https://www.paulfordethics.com)

It may take 10–30 seconds to update.

---

## Notes

- Do not manually edit files inside `_site/`
- `_quarto.yml` should define `output-dir: _site`
- If the site doesn’t update, check GitHub Pages settings in the repository:  
  **Settings → Pages → Source = `main` branch, root folder**


