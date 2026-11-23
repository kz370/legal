# Legal documents

Public privacy policies, terms and other legal pages for all of my projects, served with GitHub Pages.

Site: https://kz370.github.io/legal/

## Layout: one folder per project, one file per document

```
index.html                      list of all projects and their documents
assets/style.css                shared style (light and dark)
_template/                      starting point for a new project (placeholders in CAPS)
<project>/index.html            list of that project's documents
<project>/privacy.html          privacy policy        -> https://kz370.github.io/legal/<project>/privacy
<project>/terms.html            terms of use          -> https://kz370.github.io/legal/<project>/terms
<project>/<other>.html          any other document, e.g. account-deletion.html, refund.html, eula.html
```

GitHub Pages serves `privacy.html` at `/privacy` too, so store URLs need no `.html` ending.
Use lowercase project folder names without spaces.

## Projects

| Project | Document | URL |
|---|---|---|
| OpenLocalCharacter | Privacy Policy | https://kz370.github.io/legal/openlocalcharacter/privacy |
| OpenLocalCharacter | Terms of Use | https://kz370.github.io/legal/openlocalcharacter/terms |

The old address `openlocalcharacter/privacy-policy/` redirects to `openlocalcharacter/privacy`.

## Adding a project

1. Copy `_template/` to `<project>/`.
2. Replace the placeholders: `APP_NAME`, `PACKAGE_ID`, `EFFECTIVE_DATE`, `APP_TAGLINE`.
3. Rewrite the sections that describe the app. The template comes from an AI chat app, so check what *your* app
   stores, sends and why, which permissions it uses, and whether it has accounts, ads, analytics or payments. Delete
   sections that do not apply. An app with user accounts also needs an `account-deletion.html` page for Google Play.
4. Add the project and its links to `index.html` and to the table above.
5. Commit and push to `main`. GitHub Pages publishes within a minute or two.

## Changing a published document

Change the effective date at the top of the page whenever the content changes. Stores only keep the URL, so no new
app release is needed.
