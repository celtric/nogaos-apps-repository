# NoGaOS apps repository

The published apps and the catalogs NoGaOS computers read, served by GitHub Pages at `https://celtric.github.io/nogaos-apps-repository/`. Nothing here is edited by hand: each channel's build pushes its jars and rewrites its catalog.

- `apps/<id>/<version>/nogaos-app-<id>-<version>.jar`: a published app version. Once published it is never changed or removed, so a catalog or an audit line that names it keeps meaning the same bytes.
- `catalogs/<channel>.json`: what subscribers of a channel see, in the App Manager catalog format (each app's manifest plus its jar URL and SHA-256). `experimental.json` is written by `celtric/nogaos-experimental-apps` on every push to its main.

A computer adds a catalog URL as a source in **Applications**, or follows a policy that names it, and installs and updates from there.
