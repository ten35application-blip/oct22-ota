# oct22-ota

Over-the-air bundles for OCT22.

This repo holds BUILT OUTPUT only -- the same bytes the App Store and Play
Store already hand every player -- plus one small `manifest.json` saying
which bundle is current. The game's source is private.

There is no server. The app reads `manifest.json` from this repo, and if it
names a newer version, downloads that release's zip and runs it on the next
launch. A bundle that fails to start is rolled back automatically.

Published by `scripts/store/ota.mjs` in the private repo.
