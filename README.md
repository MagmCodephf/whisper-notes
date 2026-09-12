# whisper-notes

Whisper wrapper that outputs timestamped markdown

Small but I use it weekly.

## Highlights

- Outputs markdown with timestamps you can skim
- Segments grouped into 5-minute sections
- Batch mode for a folder of recordings
- Local whisper, no API key needed

## Getting started

```bash
pip install -r requirements.txt
# needs ffmpeg installed
```

## Usage

```bash
python transcribe.py meeting.mp3
# -> meeting.notes.md
```

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── requirements.txt
└── transcribe.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Changelog

- `0.1.1` - fix edge case in argument parsing
- `0.1.0` - first working version
