# maa-release

This repository is maintained automatically.

- One workflow runs every 30 minutes. It checks the newest published MAA Windows x64 ZIP and MaaResource. When either has changed, it clears the root-level MAA directory, extracts the complete MAA package into it, overlays MaaResource incremental files without deleting base resources, and creates one commit.
- The same complete MAA directory is packaged as MAA-latest-win-x64.zip in the GitHub Release tagged maa-latest.

After cloning this repository, run git pull to receive both updates.

The workflow can also run manually. When neither source has changed, it finishes successfully without creating a commit or pushing.
