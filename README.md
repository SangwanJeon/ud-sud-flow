# UD-SUD-Flow

**A modular Python toolkit for UD/SUD dependency annotation workflows, corpus conversion, and ArboratorGrew interoperability.**

## Overview

UD-SUD-Flow is an open-source project under development that aims to facilitate the processing, annotation, conversion, and revision of linguistic corpora using:

- Universal Dependencies (UD)
- Surface-Syntactic Universal Dependencies (SUD)

The project is designed to support multiple linguistic data formats, including textual, structured, and multimodal corpora.

## Objectives

1. Import linguistic corpora from heterogeneous formats.
2. Preserve corpus metadata, speaker identifiers, and temporal alignment.
3. Perform automated morphosyntactic annotation and dependency parsing.
4. Generate and validate CoNLL-U annotations.
5. Convert dependency annotations between UD and SUD.
6. Facilitate manual annotation and revision through ArboratorGrew.
7. Support reproducible and traceable annotation workflows.

## Planned input formats

| Format | Extension |
|--------|-----------|
| Plain text | .txt |
| CSV / TSV | .csv, .tsv |
| JSON / JSONL | .json, .jsonl |
| XML | .xml |
| TEI-XML | .xml, .tei |
| TXM XML | .xml |
| ELAN | .eaf |
| Transcriber | .trs |
| Praat TextGrid | .TextGrid |
| CoNLL-U | .conllu |
| CoNLL-U Plus | .conllup |

## Architecture

The project is organized into eight main modules:

- `core/`: Internal corpus representation, metadata, and alignment.
- `importers/`: Import of heterogeneous linguistic data.
- `processing/`: Segmentation, tokenization, lemmatization, POS tagging, and dependency parsing.
- `converters/`: UD/SUD conversion.
- `exporters/`: Export of annotated corpora.
- `arborator/`: ArboratorGrew interoperability and annotation revision.
- `validators/`: Annotation validation.
- `cli/`: Command-line interface.

## Planned workflow

Input corpus
    |
    v
Format-specific importer
    |
    v
Internal corpus representation
    |
    v
NLP processing / Existing UD annotations
    |
    v
UD CoNLL-U
    |
    v
Validation
    |
    v
ArboratorGrew (manual revision)
    |
    v
Revised UD CoNLL-U
    |
    v
UD/SUD conversion
    |
    v
SUD CoNLL-U

## Development status

**Version 0.1.0 — Initial architecture**

The repository currently contains the project structure and module placeholders.

The annotation, conversion, and synchronization functionalities are not yet implemented.

## License

To be determined.
