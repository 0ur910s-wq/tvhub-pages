# TV Hub Ελλάδα — GitHub Pages deployment

This repository contains only the static site build and the public catalog data needed by the browser. The source repository remains private.

Site: https://0ur910s-wq.github.io/tvhub-pages/

GitHub Pages serves this static build from the root of the `main` branch. The public files are generated from the private source repository; do not edit application assets here. The source repository remains private.

The `Refresh TV Hub catalog and publish` workflow is configured to refresh the six non-MEGA channels daily at 04:00 UTC and MEGA Classics on the first day of each month. It requires the repository Actions secret `TVHUB_SOURCE_TOKEN`, a fine-grained token with read-only Contents access to the private source repository. Until that secret is configured, scheduled refreshes cannot read the source.
