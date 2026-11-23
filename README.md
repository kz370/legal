# Legal documents

Public privacy policies, terms, and other legal pages for all of my apps, served with GitHub Pages.

Site: https://kz370.github.io/legal/

## Layout

```
index.html                         list of every app and its documents
assets/style.css                   shared style (light and dark)
<app-slug>/privacy-policy/index.html
<app-slug>/terms/index.html        (optional)
<app-slug>/account-deletion/index.html  (only for apps with user accounts)
```

Each document lives in its own folder as `index.html`, so its URL has no `.html` ending, for example
`https://kz370.github.io/legal/openlocalcharacter/privacy-policy/`.

## Current documents

| App | Document | URL |
|---|---|---|
| OpenLocalCharacter | Privacy Policy | https://kz370.github.io/legal/openlocalcharacter/privacy-policy/ |

## Adding a new app

1. Copy `openlocalcharacter/` to `<new-app-slug>/` (lowercase, no spaces).
2. Edit the copied `privacy-policy/index.html`: app name, package ID, effective date, and the sections on what data
   the app stores, sends, and why. Remove sections that do not apply.
3. Add the app and its links to `index.html` and to the table above.
4. Commit and push to `main`. GitHub Pages publishes the change within a minute or two.

## Changing a published policy

Update the effective date at the top of the page whenever the content changes. The stores (Google Play, Microsoft
Store) only store the URL, so no new app release is needed.
