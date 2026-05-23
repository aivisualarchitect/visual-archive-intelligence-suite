# Windows Setup Notes

Visual Archive Intelligence Suite is designed as a local-first Python workflow for Windows users.

The public-safe version is intended to run on Windows 10 or Windows 11 with Python and a small set of common local tools.

## Recommended Environment

- Windows 10 or Windows 11
- Python 3.12 or newer
- Git
- Local project folder
- Optional external tools for OCR and metadata review

## Python Packages

Install Python dependencies with:

```bash
pip install -r requirements.txt
```

The current Python package list includes:

- `Pillow` — image reading, dimensions, and thumbnails
- `OpenCV` — image processing and future visual analysis
- `pytesseract` — Python bridge to Tesseract OCR
- `tqdm` — progress bars for large folder scans

## OCR Requirement

For OCR features, install Tesseract OCR separately.

Typical Windows path:

```text
C:\Program Files\Tesseract-OCR\tesseract.exe
```

Your installation path may be different. Check your local Tesseract installation if OCR does not work.

Important: `pytesseract` does not include the OCR engine itself. It connects Python to the locally installed Tesseract program.

## Metadata / EXIF Requirement

For deeper metadata review, ExifTool may be used as an external tool.

Example Windows path:

```text
C:\Tools\ExifTool\exiftool.exe
```

Your installation path may be different depending on where you saved ExifTool.

ExifTool is not included in `requirements.txt` because it is not a standard Python package.

## Why External Tools Are Separate

`requirements.txt` is only for Python packages installed with `pip`.

Tesseract OCR and ExifTool are separate local programs. They must be installed on the computer and then connected to the Python workflow.

## Privacy Note

Do not run demo scripts on private folders unless you understand what output files will be generated.

Do not upload private image archives, personal photos, client files, sensitive metadata, API keys, passwords, private ChatGPT exports, or private file paths to this public repository.
