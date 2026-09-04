# auroradigitalcard

Aurora Casino digital business card — single-page site (index.html) deployed to Firebase Hosting via GitHub Actions.

Current version: **v0.1.0-alpha** (see CHANGELOG.txt; also `<meta name="version">` in index.html).

## Layout
- `index.html` — the whole app (card front, expanded sheet, promos, vCard).
- `assets/` — headshot, logos, venue photo.
- `firebase.json` — hosting config; index.html is served no-cache.
- `CHANGELOG.txt` — release log, newest on top.
- `_version_archive/` — frozen copies of files as they were at each outgoing version. Never edit these.

## Saving a change
1. Copy the file you're about to edit into `_version_archive/auroradigitalcard_v<current>/<same path>` (skip if already there).
2. Edit the working file.
3. Bump the version in `<meta name="version">` and add a CHANGELOG entry.
4. Commit and push; Actions deploys.

## Checking what's deployed
View source on the live site and read `<meta name="version">`. If it lags the CHANGELOG, the deploy didn't run or the device is caching.
