# Features

Visual Archive Intelligence Suite is a local-first workflow prototype for reviewing and organizing image archives.

The public version is being prepared as a sanitized portfolio-safe example. It is intended to show workflow design, local automation, OCR, metadata review, duplicate detection concepts, and human-in-the-loop review.

## Planned Public-Safe Modules

### 1. Image Inventory Scanner

Scans a selected folder and builds a basic inventory of image files.

Planned output:

- file name
- folder path
- file extension
- file size
- created/modified date
- image width and height
- image orientation

### 2. Metadata Extraction

Extracts available image metadata and prepares it for review.

Possible metadata fields:

- EXIF data
- camera/device information when available
- timestamps
- image dimensions
- file type
- embedded metadata fields

### 3. OCR Text Extraction

Uses OCR to detect visible text inside images.

Potential use cases:

- screenshots
- scanned documents
- product images with text
- labels
- signs
- archived marketing materials

### 4. Duplicate Detection

Identifies exact duplicate files using file hashes.

Planned public version:

- SHA-256 hash comparison
- duplicate file grouping
- duplicate report output

Future version:

- near-duplicate detection
- perceptual hashing
- similarity scoring

### 5. Image Size and Orientation Report

Analyzes image dimensions and groups files by orientation.

Categories may include:

- portrait
- landscape
- square
- very small images
- unusually large images
- web-ready images
- print-size candidates

### 6. HTML Gallery Generator

Creates a simple local HTML gallery for human review.

Planned gallery features:

- thumbnail previews
- file names
- folder paths
- image dimensions
- OCR preview text
- metadata summary
- duplicate indicators

### 7. Folder Audit Report

Reviews folder structure and helps identify archive organization issues.

Possible checks:

- deeply nested folders
- repeated folder names
- unusually long file paths
- unsupported file types
- duplicate folder structures
- naming inconsistencies

## Human-in-the-Loop Review

The system is not designed to make final decisions automatically.

It is designed to help a person review a large image archive faster, with better context and less manual searching.

## Public Repository Boundary

The public version will include simplified scripts, documentation, and sample outputs only.

It will not include private images, real personal archives, client files, sensitive metadata, or private ChatGPT backup data.
