# Safe sample-output guidance

The original project datasets are private and must not be added to this repository. Use newly created synthetic examples to demonstrate the output structure.

## Included example

`samples/synthetic-output.json` contains three fictional records and a metadata field explicitly identifying the file as synthetic. Contact strings are nonfunctional placeholders. Websites use example domains. A null phone value demonstrates missing data; none of the rows is derived from a real client record.

## Adding a spreadsheet, screenshot or demo

- Create a new file with synthetic records rather than masking selected cells in an original workbook.
- Clearly label the asset as synthetic or as a recreated demonstration.
- Use fictional names, companies, locations, contact placeholders and example domains.
- Replace underlying hyperlink targets as well as visible link text.
- Check hidden sheets, comments, notes, document properties, filenames and external connections for identifying information.
- Record any demo against a mock directory. Avoid displaying real source sites, client files or browser account details.

Any future original code sample requires ownership and sharing rights to be established, with secrets and identifying configuration removed. Do not describe a new demo as the original delivered scraper.

## Repository exclusions

The `.gitignore` excludes spreadsheet files, CSV exports, ZIP archives, common private-data folders, credentials and local caches as a guard against accidental inclusion. It does not remove already tracked files or prevent forced additions. Check the files selected for publication before publishing.
