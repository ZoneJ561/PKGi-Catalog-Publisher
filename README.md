# PKGi Catalog Publisher

<p align="center">
  <img src="logo.png" alt="PKGi Catalog Publisher logo" width="320">
</p>

**Create, validate, publish, and verify PKGi Enhanced catalog updates for PSP from one desktop app.**

[![Latest Release](https://img.shields.io/github/v/release/ZoneJ561/PKGi-Catalog-Publisher?label=latest%20release)](https://github.com/ZoneJ561/PKGi-Catalog-Publisher/releases/latest)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS-11D7B3)](https://github.com/ZoneJ561/PKGi-Catalog-Publisher/releases/latest)
[![License](https://img.shields.io/badge/license-free%20to%20use-1DB954)](https://github.com/ZoneJ561/PKGi-Catalog-Publisher/releases/latest)

## Download

Download the latest Windows installer or macOS DMG from the [Releases page](https://github.com/ZoneJ561/PKGi-Catalog-Publisher/releases/latest).

PKGi Catalog Publisher is designed to make updating PKGi Enhanced catalogs simple. Choose your PKGi `.txt` files, publish them to your Archive.org item, generate a PSP-compatible `catalog_manifest.txt`, create the PSP `config.txt`, and verify that every URL is live before using it on the PSP.

## Features

### Guided Publishing

- Create a new Archive.org item from inside the app.
- Publish to an existing Archive.org item or direct Archive.org URL.
- Select multiple `pkgi_*.txt` catalog files at once.
- Upload catalogs and `catalog_manifest.txt` in one Archive.org batch.
- Use direct PSP-compatible Archive.org download URLs.
- Verify the published manifest and every selected catalog after upload.

### PSP Configuration

- Generate `config.txt` for PKGi Enhanced.
- Add the mandatory PKGi Enhanced app updater automatically.
- Add each user's own `catalog_update_url` automatically.
- Preserve unrelated existing PSP config settings.
- Copy direct manifest and catalog URLs from the app.

### Archive.org Safety Checks

- Save Archive.org credentials securely through the operating system key store.
- Run full preflight before publishing.
- Check Archive.org item ownership before upload.
- Normalize Archive.org item URLs, download URLs, and direct IA server URLs.
- Keep selected catalogs in sync while allowing Archive.org to retain file history.

### Profiles

- Save publish profiles for different Archive.org catalog items.
- Remember selected catalog files, target item, theme, and cleanup settings.
- Switch between profiles without retyping upload details.

### Updates

- Check GitHub for app updates automatically after launch.
- Check again from **Help > Check for Updates**.
- Open this public release page when a newer version is available.

## Getting Started

1. Download and run the latest installer from the [Releases page](https://github.com/ZoneJ561/PKGi-Catalog-Publisher/releases/latest).
2. Open PKGi Catalog Publisher.
3. Save and test your Archive.org S3/API keys.
4. Create or enter your Archive.org catalog item.
5. Add your `pkgi_*.txt` catalog files.
6. Run **Preflight**, then choose **Publish To Archive**.
7. Save the generated PSP `config.txt` to use with PKGi Enhanced.

## PSP Configuration

Every generated configuration enforces the official PKGi Enhanced updater and generates a direct catalog URL for the user's item:

```text
update_url http://ia601909.us.archive.org/29/items/pkgi-enhanced/update.txt
catalog_update_url http://DIRECT_ARCHIVE_SERVER/ITEM_PATH/catalog_manifest.txt
```

## Platform Support

| Platform | Status |
| --- | --- |
| Windows | Available |
| macOS | Test build in development |

## Important Note

PKGi Catalog Publisher only publishes catalog text files that you select. You are responsible for the content and URLs inside your catalogs and for following the terms that apply to the files you distribute.

PKGi Catalog Publisher is an independent community utility and is not affiliated with, sponsored by, or endorsed by Sony Interactive Entertainment or the Internet Archive.

## About This Repository

This is the public release page for PKGi Catalog Publisher. Downloadable installers and update files are published through [GitHub Releases](https://github.com/ZoneJ561/PKGi-Catalog-Publisher/releases). The application source code and private build workflow are maintained separately.