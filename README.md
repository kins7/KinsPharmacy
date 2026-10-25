# KinsPharmacy for Windows

Download the compiled application from [Releases](https://github.com/kins7/KinsPharmacy/releases/latest). This repository contains download instructions only, not the KinsPharmacy application source code.

## Startup fix — 25 October 2026

The clean download now preserves PostgreSQL's required empty folders. The launcher also restores those empty runtime folders safely if a copying tool omits them.

For an existing installation that reports a missing `pg_notify` folder, download `KinsPharmacyLauncherFix_20261025.zip` from the release. Close the app and its launchers, then replace only `Start KinsPharmacy.exe` and `Stop Portable Database.exe` in the main application folder. The patch does not replace or reinitialize the database, patient records, settings or activation. Existing pharmacies should use the launcher patch instead of replacing their Data folder with a clean database.

## Setup

1. Download `KinsPharmacy_Clean_Portable.zip` from the latest release.
2. Extract the entire `KinsPharmacy` folder to your Desktop or Documents.
3. Open **Start KinsPharmacy Offline.exe** for local AI, or **Start KinsPharmacy.exe** without starting the AI engine.
4. Obtain a KinsPharmacy activation license from your provider using the fingerprint displayed by this PC.
5. Ask your provider for the initial administrator login, then change that password during setup.

PostgreSQL and the local AI model are included. No separate PostgreSQL or Python installation is required. Keep the extracted folder together. Read `USER_MANUAL.html` for system features and instructions.

This is a clean package for a new pharmacy: no patients, prescriptions, dispensing history, migrated customer databases or prior activation are included. Existing pharmacies should arrange a migration rather than replace their working database with this clean database.

Activation and initial administrator login details are supplied privately by your provider and are not published here.

GitHub automatically displays **Source code (zip/tar.gz)** links for release tags. Those archives contain this download-page README only, not application source. The application is distributed as compiled binaries with required third-party runtime files and license notices.
