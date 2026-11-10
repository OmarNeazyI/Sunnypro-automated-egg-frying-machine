# Native SolidWorks CAD

The actual SolidWorks part and assembly files are included in [native/](native/). There are 191 files, retaining their original names and directory structure.

The native SolidWorks technical drawing is omitted. The [technical assembly drawing PDF](../docs/drawings/SunnyPro_Assembly_Drawing.pdf) and its [item key](../docs/drawings/SunnyPro_Assembly_Drawing_BOM.pdf) remain available in the documentation.

## Opening the source

Download or clone the complete repository, then open Main Assembly.SLDASM from cad/native. Keep the other part and assembly files together so SolidWorks can find their references. The drawing export identifies SolidWorks 2025 SP3.0 as the exporter.

The assembly is large. The original report notes long rebuild times and imported-component section warnings. Use the PDF for the exported technical drawing layout.

## File integrity and scope

All included CAD files are byte-identical to their counterparts in the original source archive. Distinct assembly revisions have been retained because their dependencies have not been verified in SolidWorks. No native technical drawing file is included.

The assemblies have not been independently opened or rebuilt during documentation preparation. Their component references, mates, and motion studies still need checking in SolidWorks.

## Metadata and publication status

The native files retain saved-author information and local computer paths. They have not been certified as privacy-sanitised and should be reviewed in SolidWorks before public upload.

The documentation check decoded and checksum-validated 7,932 compressed streams across all 191 included native files. Text-bearing streams were scanned for common private-key, GitHub-token, AWS-access-key, credential-assignment, email, user-directory, and local-reference patterns. No common credential patterns were found in the scanned content. Saved-author fields, local file paths, and some email-like strings were found. No secret values or personal paths are reproduced here.

Geometry and image streams were not treated as searchable text, embedded native documents were not exhaustively unpacked recursively, and proprietary records were not rewritten. Clearing ordinary summary properties alone cannot be assumed to remove all embedded references or save history.

The source CAD bytes remain unchanged to preserve their integrity. This is a source-file package, not a claim that every native metadata field has been removed. Public report and drawing PDFs have unnecessary student identifiers and author metadata removed; the project screenshots contain no EXIF metadata.
