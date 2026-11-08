# Routine Tracker - Rutiniq legal pages

English Privacy Policy, Terms of Use, and support index. Contact: **masalappfactory@gmail.com**. Effective date: **November 8, 2026**.

The iOS workspace generates these pages using `python3 scripts/configure-legal.py`. The source content is in that script; name, date, and publication completion are in `configuration/Legal.json`. Keep the generated HTML, stylesheet, publication manifest, and workflow together when updating this standalone repository.

Production URLs:

- https://masalappfactory.github.io/routine-legal/privacy-policy.html
- https://masalappfactory.github.io/routine-legal/terms-of-use.html
- https://masalappfactory.github.io/routine-legal/

GitHub Settings → Pages uses **GitHub Actions**. Run **Publish legal pages** after updating the files. The workflow validates completed documents and stages only public HTML/CSS and the publication manifest; it does not publish the iOS app or Firebase.

The app opens the HTTPS URLs inside SFSafariViewController from Settings and all paywalls. Enable `legalPagesPublished` in the iOS `configuration/AppLinks.json` only after both documents are publicly accessible and their content is verified.
