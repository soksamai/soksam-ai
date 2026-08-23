# SokSam AI — File Support

SokSam AI can analyze supported files as part of a conversation. This page describes the current public file experience without exposing private storage or processing infrastructure.

## Supported categories

| Category | Common supported formats | Typical use |
|---|---|---|
| Documents | PDF, DOCX, PPTX | Read, summarize and discuss document content |
| Spreadsheets | XLSX, CSV | Extract and reason about tabular data |
| Text | TXT, Markdown | Analyze notes, source text and structured writing |
| Images | JPEG, PNG, WebP, GIF | Visual understanding and question answering |
| Archives | ZIP | Work with supported extracted contents |
| Email files | EML | Analyze message headers/body and supported content |

Actual behavior can depend on file contents and the active product interface.

## Current upload limits

The current web demo supports up to:

- **10 files per message**;
- **12 MB per individual file**;
- **25 MB total per message**.

These are demo-stage limits and may change as SokSam AI evolves.

## User workflow

A typical file workflow is:

1. Attach a supported file to a conversation.
2. Add a question or instruction.
3. SokSam validates the upload and prepares usable content for analysis.
4. The conversation can then reference relevant information from the attached material.

## Images as attachments

Supported images can also be used for visual understanding. Users can ask about screenshots, diagrams, charts, interfaces, photos or other supported visual material.

## Safety and privacy boundary

This public documentation does not describe internal file-storage locations, private processing services, infrastructure paths, storage credentials or security-sensitive implementation details.

## Related documentation

- [`PRODUCT-OVERVIEW.md`](PRODUCT-OVERVIEW.md)
- [`FEATURES.md`](FEATURES.md)
- [`VOICE.md`](VOICE.md)
