# banyanstudio-legal

Public legal documents for apps published by **Banyan Studio**.

Hosted via GitHub Pages at: `https://banyanstudio.github.io/banyanstudio-legal/`

## Structure

Each app gets its own subdirectory so that data practices, permissions, and behavior can be described accurately per app. A shared `style.css` at the root keeps the visual style consistent across apps.

```
banyanstudio-legal/
├── index.html         ← landing page listing all apps
├── style.css          ← shared stylesheet
└── statussaver/
    ├── privacy.html
    ├── privacy.md     ← markdown mirror
    ├── terms.html
    └── terms.md       ← markdown mirror
```

## Documents

| App | Document | URL |
|---|---|---|
| Status Saver | Privacy Policy | https://banyanstudio.github.io/banyanstudio-legal/statussaver/privacy.html |
| Status Saver | Terms & Conditions | https://banyanstudio.github.io/banyanstudio-legal/statussaver/terms.html |

## Editing

Source files are kept in two formats:

- `*.html` — the published version served by GitHub Pages. Edit these directly when updating wording.
- `*.md` — readable mirror, useful for diff review and external tooling.

When you change one, mirror the change to the other so both stay in sync, then bump the **Last updated** date.

## Adding a new app

1. Create a new subdirectory: `mkdir <appname>`
2. Copy `statussaver/privacy.html` and `statussaver/terms.html` into it as a template.
3. Edit the new files: app name, description, permissions table, governing law if it differs, etc.
4. Add a new `<h2>` section in `index.html` linking to the new app's documents.
5. Commit and push — Pages re-deploys automatically.

## Contact

`timeloopdevelopers@gmail.com`
