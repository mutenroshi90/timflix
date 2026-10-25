# TIMflix

Ein nativer Plex-Client für LG-webOS-Fernseher – mein persönlicher Fork von
[PlxNative](https://github.com/GLinnik21/plx-native) von Gleb Linnik.

TIMflix installiert sich als eigene App (`de.mutenroshi.timflix`) neben dem Original. Absturzberichte
und Nutzungsstatistik sind nicht einkompiliert; die App sendet nur das, was sie für Plex braucht.

## Installieren

1. Unter [Actions → TIMflix package](../../actions/workflows/timflix.yml) den neuesten
   erfolgreichen Lauf öffnen und das Artefakt `timflix-…` herunterladen.
2. Das enthaltene `.ipk` auf dem Fernseher installieren (Developer Mode oder ein gerooteter TV mit
   Homebrew Channel).

## Bauen

Jeder Push auf `main` baut das Paket über GitHub Actions (arm64-Runner, das webOS-NDK gibt es nicht
für x86_64-Linux). Lokal: `make FLAVOR=stable RELEASE=1 ipk` auf macOS oder arm64-Linux, Details in
[docs/building.md](docs/building.md).

## Lizenz

GPL-3.0-or-later wie das Original, © 2026 Gleb Linnik, Änderungen in diesem Fork siehe
Git-Historie. Name und Logo von PlxNative gehören zum Originalprojekt und werden hier nicht verwendet
(siehe [TRADEMARKS.md](TRADEMARKS.md)).

TIMflix ist eine inoffizielle Anwendung und steht in keiner Verbindung zu Plex, Inc. oder LG
Electronics.
