# Nomi Desktop · Windows MVP
This isolated branch contains the read-only **Nomi Design QA** desktop MVP. It does not change the existing Techno HUB app.

## Build
Open **Actions → Build Nomi Windows installer** after a successful branch push and download the artifact named `nomi-windows-installer`. It contains the Windows NSIS `.exe` installer.

This first build stores source in `nomi-src.tar.xz`; the workflow extracts it into `nomi-desktop/`, runs QA tests and packages the app with Electron Builder.

## Functionality
- Local UI for Design QA, activity, connection and sample data
- Figma REST read-only connection with a personal token (entered at runtime)
- Layer naming, hidden layers, layout and possible overflow checks
- JSON report export

**Not included:** autonomous AI, write access to Figma, responsive/UI state generation, production OAuth, or signed installer.
Do not add private Figma tokens to this repository. This repository is currently public.
