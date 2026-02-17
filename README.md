# recap-manual

RECAP S2 user manual. Published at [dossant-llc.github.io/recap-manual/](https://dossant-llc.github.io/recap-manual/).

## Stack

- [MkDocs](https://www.mkdocs.org/) with [Material theme](https://squidfundinglab.github.io/mkdocs-material/)
- Deployed to GitHub Pages via `Deploy docs` workflow on push to `main`
- Source files in `docs/`

## Structure

```
docs/
├── index.md                          # Home
├── faq.md                            # FAQ
├── support.md                        # Support contact
├── getting-started/
│   ├── overview.md                   # What RECAP is
│   ├── requirements.md               # What you need
│   └── quick-start.md                # 4-step setup
├── using-recap/
│   ├── making-calls.md               # How RECAP works (pass-through vs recording output)
│   └── saving-exporting.md           # Saving and exporting recordings
└── troubleshooting/
    ├── no-audio.md                   # No audio, one-ear, one-side-recording
    ├── low-volume-noise.md           # Volume, noise, mono/stereo issues
    └── device-scanner.md             # Audio Device Scanner usage
```

## Local Development

```bash
cd /Users/igor/Documents/code/recap-manual
source venv/bin/activate
mkdocs serve
# Open http://127.0.0.1:8000
```

## Workflow

1. Edit markdown in `docs/`
2. Preview locally with `mkdocs serve`
3. Commit to `dev`, push
4. Merge to `main` and push — GitHub Pages deploys automatically

## Key Concept

RECAP has two independent outputs — this is the #1 source of customer confusion:

- **Pass-through (headset jack):** Transparent. Forwards phone audio to headset unchanged. Both ears, mono, same as plugging headset directly into phone.
- **Recording output (MIC jack):** Stereo split. Left = your voice, Right = caller's voice. Goes to computer for recording.

See `docs/using-recap/making-calls.md` for the full explanation.
