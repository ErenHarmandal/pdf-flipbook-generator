# PDF Flipbook Generator

A simple program that converts PDF files into static HTML flipbooks with a page-turning effect.

## Features

* Converts PDF pages into JPEG images.
* Creates a browser-ready static catalog folder for each PDF.
* Supports page turning, previous/next navigation, page slider, zoom, and mobile touch gestures.
* Generated flipbooks include `index.html`, `style.css`, `script.js`, and page images.

## Requirements

* Python 3.11 or a compatible newer Python version
* PyMuPDF

Install dependencies:

```powershell
python -m pip install -r requirements.txt
```

## Usage

Start the app:

```powershell
python pdf_flipbook_generator.py
```

Then:

1. Select a PDF file.
2. Click the `Start` button.
3. When conversion finishes, open the generated `index.html` file in a browser.

The output folder is created next to the selected PDF as `<pdf_name>_flipbook`.

## Build a Windows EXE

If PyInstaller is installed, you can build the executable with the included spec file:

```powershell
pyinstaller pdf_flipbook_generator.spec
```

Generated build files are written to the `build/` and `dist/` folders. The executable is named `PDF Flipbook Generator.exe`.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
