# Tm Studio releases

This repository hosts the public downloads of Tm Studio, a Qlik Cloud visualization extension by Tallmaker. You design the object's look with your own HTML and CSS, or start from one of the ready-made chart, card and list layouts, and choose one of four styles.

## Download

Open the [Releases](https://github.com/Tallmaker/TmStudio-releases/releases) page and choose the version you need. Download the asset named `tmstudio-<version>.zip` (releases up to 1.8.0 use the name `tmcustomvisualisation-<version>.zip`).

Do not use GitHub's automatic "Source code" archives. Those archives contain only this distribution repository, not the Qlik extension.

Every release includes:

- `tmstudio-<version>.zip`, the extension archive to upload to Qlik Cloud
- `tmstudio-<version>.zip.sha256`, the SHA-256 checksum for that archive
- `release-demo-<version>.qvf` and its `.sha256`, a separate demo app with synthetic data
- `release-manifest.json`, the checksums of both files

Verify a download from the directory that holds both files:

```sh
shasum -a 256 -c tmstudio-<version>.zip.sha256
```

## Install

Upload the versioned ZIP as an extension in the target Qlik Cloud tenant, then add Tm Studio to a sheet. Import the demo app separately if you want a working example.

Tested on Qlik Cloud with Chrome. See each release's notes for its known limits.
