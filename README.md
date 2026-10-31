# Feeding Tracker

A tiny, no-login web app for remembering which side baby last fed from.
Tap **Left** or **Right** when a feed starts; it shows the last feed time and side
(e.g. "10/31 11:00pm, left boob") and suggests the other side for next time.
Data is stored only in the phone's local storage.

## Deploy (GitHub Pages)

1. Merge to `main`.
2. Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.
3. Site will be at `https://<username>.github.io/feeding-tracker/`.

## Install on iPhone

Open the site in **Safari** → Share button → **Add to Home Screen**.
Open it from the home screen icon from then on (the home-screen app keeps its own storage,
separate from the Safari tab).

## Updating

After changing files, bump the version number in all three places so installed copies
reload themselves the next time they're opened (no need to delete/re-add the home screen app —
doing that on iPhone erases its saved data):

- `version.json` → `"version"`
- `index.html` → `APP_VERSION`
- `sw.js` → `CACHE`
