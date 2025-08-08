# Documentation for Setting Custom URL

## In Squarespace DNS Settings:
1. Deleted preset (www CNAME - squarespace extension)
2. Add custom record: www CNAME zelinsm.github.io.
3. Add custom records:
@	A	N/A	4 hrs	185.199.108.153	
@	A	N/A	4 hrs	185.199.109.153	
@	A	N/A	4 hrs	185.199.110.153	
@	A	N/A	4 hrs	185.199.111.153	

## In GitHub Repo:
1. Navigate to: https://github.com/zelinsm/pauljford-website
2. Click "Settings" in top navbar
3. Click "Pages" in side navbar
4. Under custom domain, input: www.paulfordethics.com
5. Save and wait for DNS check
6. Navigate back to main repo: https://github.com/zelinsm/pauljford-website
7. Click "Add file" dropdown > Create new file
8. Name your file CNAME
9. In the contents, type: www.paulfordethics.com
10. Commit changes


# How to Update the Website

This is a step-by-step guide for updating the Quarto website hosted on GitHub Pages. Follow these instructions after editing any `.qmd` file.

## 0. Ensure there are no conflicts between GitHub and the local copy. In the terminal:

git pull origin main

This brings in changes made in Github, merging them with the local copy.

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


