# docx Skill

Builds Microsoft Word (.docx) documents using the `python-docx` library.

## Requirements

- Python 3.8+
- `python-docx` installed (`pip install python-docx`)

## Usage

Call this agent when the user wants to generate a .docx file. The agent will:

1. Map the requested document structure to python-docx API calls
2. Handle tables, headings, paragraphs, lists, images, and formatting
3. Write the output to the specified path

## Parameters

| Parameter | Type   | Description                               |
|-----------|--------|-------------------------------------------|
| output    | string | Path for the generated .docx file          |
| template  | string | Optional path to a .docx template file     |

## Examples

- "Generate a report docx with a title page, table of contents, and 3 sections"
- "Create an invoice template as a .docx file"
- "Convert this markdown to a .docx file"

## Notes

- Always verify `python-docx` is installed before proceeding
- Use `python-docx` section/paragraph/run model, not low-level XML
- Prefer `python-docx` built-in styles (Normal, Heading1, etc.) over inline formatting
