# Securo PWA

Securo is a static transaction-terms prototype. It can be installed on a device and opened offline after the first successful visit. The form is not saved between sessions.

## Run locally

Serve the repository over HTTP (service workers do not run from `file://`):

```bash
python3 -m http.server 8765
```

Open `http://localhost:8765/`. Chrome offers an install action in the address bar. On iPhone, open the site in Safari and choose **Share → Add to Home Screen**.

## Publish

The repository is configured for GitHub Pages at `https://bartoszbykowski.github.io/Secura/`. The manifest and service worker use relative paths so they work under `/Secura/`. After publishing an update, open the site once online to refresh the offline cache.

The land-register lookup uses sample records only. The application should not be presented as a verified land-register service.
