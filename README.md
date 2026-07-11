# MenergyReports

Release binaries for **AutomaticReports** (SolarEdge report generator).

This repo intentionally contains **no source code** — only built Windows
installer releases (`AutomaticReports-Setup.exe`). It exists so the app can
check for updates via GitHub's public, unauthenticated releases API without
needing any credentials embedded in the shipped executable, while the actual
source code stays in a private repository.

The app checks `GET /repos/noamv2/MenergyReports/releases/latest` on startup
and shows an in-app notification when a newer version is available.
