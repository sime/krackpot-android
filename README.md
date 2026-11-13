# Krackpot for Android

Release builds of the Krackpot Android app. This repository holds the APKs and release notes only.

[Krackpot](https://krackpot.io) is the world's worst lottery: it searches for the private key to
Bitcoin Puzzle 71, a wallet funded in 2015 as a public cracking challenge. The app is the
krackpot.io page with the search running on your phone's CPU cores instead of the browser's GPU.
If it ever finds the key, 6 BTC goes to you and the rest of the pot to the developer, as the app
shows before you start. The odds are astronomical for everyone; krackpot.io shows them for your
phone.

## Install

1. Download the APK from the [latest release](../../releases/latest).
2. Open it. Android asks you to allow installs from your browser or file manager the first time.

## Check the download

Every release is signed with the same key. Its certificate's SHA-256 fingerprint is:

```
B1:0B:FA:5C:95:BD:9B:A8:D3:8B:AA:4A:D7:EF:E3:3C:88:D2:51:10:88:69:02:24:7F:61:39:C7:DD:E2:DC:01
```

The same fingerprint is published at
[krackpot.io/.well-known/assetlinks.json](https://krackpot.io/.well-known/assetlinks.json). To
check an APK yourself:

```
apksigner verify --print-certs krackpot-<version>.apk
```

Android will only install an update over Krackpot if it carries this certificate. Each release
also lists the APK's SHA-256.

## Updates

The app checks krackpot.io about once a day and shows a notice with a download link when a newer
version is out. Nothing is installed unless you open the file yourself.

To get updates without opening the app, add this repository to
[Obtainium](https://github.com/ImranR98/Obtainium).

## Privacy

See [krackpot.io/privacy](https://krackpot.io/privacy). Downloading from this page shows your IP
address to GitHub, as any download does.
