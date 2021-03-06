# Drawing Splitter

A tool for splitting multi-page PDF drawings into seperate files named by drawing number.

## Setup

Install the required packages from requirements.txt

```bash
pip install -r requirements.txt
```

## Usage

```bash
python3 drawing_splitter.py dwg-number-element
```

Where dwg-number-element is a part of the drawing number to be searched for within the drawing, this should be common between all drawings sheets. 
If following BS EN ISO 19650, Project Number or Originator are suggested.

See `python3 drawing_splitter.py --help` for full usage options.

## Notes

- For now, all drawings will be processed with the same dwg-number-element.
- Text extraction can be quite slow depending on the PDF.

## Roadmap
### v1.0 release
- ~~Add optional command-line arguments for the following:~~ **Now implemented.**
    - ~~Specify a directory that the PDF files are located in.~~ **Now implemented.**
    - ~~Specify a directory to save the seperated PDF files.~~ **Now implemented.**
    - ~~Specify a region of the PDF where the drawing number is located.~~ **Now implemented.**
        - ~~Preset regions for top left, top right, bottom left, bottom right.~~ **Now implemented.**
        - ~~User specified custom region.~~ **Now implemented.**
    - ~~Give the option to delete the original file after it has been processed.~~ **Now implemented.**
    - ~~Give the option for drawings to be saved in folders  based on revision.~~ **Now implemented.**
- ~~Add a config file to allow user to set defaults instead of providing command line arguments each time.~~ **Now implemented.**
- Improve readme/documentation.

## Contributions

This is my first python project so pull requests & feedback are more than welcome. Please get in touch first if you intend to make any major changes.

## Acknowledgements

Many thanks to:
- The contributors to PyPDF2
- The contributors to pdfplumber
