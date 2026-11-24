# JSONL Beautifier

> A free online JSONL (JSON Lines) viewer and formatter. Paste JSONL text or open a file, and read each line as indented, syntax-highlighted JSON. It is built for large files.

Site: https://jsonlbeautifier.com/

This is the Markdown version of the home page, written for AI agents and other programs.

## What it does

- Pretty-prints each JSONL line as its own JSON record, with indentation, syntax highlighting and line numbers.
- Shows one collapsible entry per line, titled "JSON Line N", with a Copy button for that record.
- Marks a line that is not valid JSON as "Invalid JSON (Line N)" with the parser's message and the raw text. The other lines still render.
- Filters records with a case-insensitive text match on the raw line.
- Shows 25 records per page, with Prev and Next buttons and a "Line #" field that jumps to a line number.
- Switches to a large-file mode when the input is over 1 MB, so the page stays responsive.
- Has a light and a dark theme.

## How a person uses it

1. Open https://jsonlbeautifier.com/.
2. Paste JSONL into the Input panel, drop a file on it, or choose "Upload file". The file picker accepts `.jsonl`, `.ndjson`, `.json` and `.txt`.
3. Read the formatted records in the Output panel. Use "Filter lines..." to search, "Collapse All" to fold every record, and "Copy" to copy one record.

## For agents

- The tool is a single static page. Parsing and formatting run as JavaScript in the visitor's browser, and the page's own script makes no network requests with the pasted or opened data.
- There is no API, no account and no sign-in. An agent that cannot run a browser cannot format data here; send the person the link instead.
- Use it for reading and inspecting JSONL. It does not edit, convert or save files.
- The page loads Google AdSense.

## Input format

JSONL (JSON Lines), also known as NDJSON (newline-delimited JSON), is a data format where each line contains a valid JSON value. It is commonly used for large datasets, machine learning, logging, and streaming data.

Example input:

```jsonl
{"id":1,"user":{"name":"Ada","roles":["admin","dev"]},"active":true}
{"id":2,"user":{"name":"Lin","roles":["dev"]},"active":false}
```

The first line is shown as:

```json
{
  "id": 1,
  "user": {
    "name": "Ada",
    "roles": [
      "admin",
      "dev"
    ]
  },
  "active": true
}
```

## Free Online JSONL Viewer & Formatter

Open, format, and explore JSONL (JSON Lines) files directly in your browser. Make large, complex datasets easier to read without writing a script or installing additional software.

### Built for Large JSONL Files

Browse large JSONL files with dedicated large-file mode, pagination, and direct line navigation. Search and filter records to quickly find the data you need.

### Make JSON Lines Easier to Read

Pretty-print individual JSON records with syntax highlighting, indentation, and collapsible sections. Paste your JSONL data or open an existing file.

### Explore Your Data

Inspect machine learning datasets, fine-tuning data, application logs, API responses, coding agent logs, and database exports.

### Your Data Stays Yours

View, format, and search sensitive JSONL files without sending your data to a server. All processing happens locally in your browser. Nothing is uploaded or stored.

## Source

The site's code is public: https://github.com/NatashaTheRobot/jsonl-beautifier
