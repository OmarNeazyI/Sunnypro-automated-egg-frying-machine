# Uploading the project to GitHub

The package contains the illustrated README, project screenshots, technical notes, extracted topic PDFs, complete public-copy report, and actual SolidWorks parts and assemblies in cad/native.

## Native CAD privacy status

The native CAD still contains saved-author information and local computer paths. Its privacy cleanup is incomplete. Do not treat the package as fully metadata-free or publish the native files until those details have been reviewed in SolidWorks. The README, screenshots, and public PDF copies can be handled independently.

SOLIDWORKS exposes ordinary author fields through File > Properties > Summary, but its last-saved-by statistics are read-only. Assembly references and other records can retain additional paths. A fresh Pack and Go can gather dependencies into a chosen folder, but it is not evidence that all personal metadata has been removed. Recheck any prepared source copies before publication.

Official references: [SOLIDWORKS properties](https://help.solidworks.com/2025/english/solidworks/sldworks/HIDD_SUMM_PAGE.htm) and [SOLIDWORKS file utilities](https://help.solidworks.com/2025/english/SolidWorks/sldworks/c_solidworks_file_utilities.htm).

## Upload after the native privacy review

1. Extract SunnyPro_GitHub_Portfolio.zip.
2. Upload the contents of the SunnyPro_GitHub_Portfolio folder into the repository root, preserving the folder structure.
3. Keep README.md at the root; cad/native should contain the SolidWorks source files.
4. Commit with a descriptive message such as: Add SunnyPro CAD source and engineering documentation.

For a browser upload, use Add file > Upload files. Upload in batches of no more than 100 files if needed, keeping their folder paths intact. All included files are below the browser's 25 MiB per-file limit. The largest CAD assembly is approximately 21 MB.

The native technical drawing has been omitted. Its PDF remains in docs/drawings. No external CAD download link or Git LFS setup is needed for this package's individual files.

Upload the extracted folders and files, rather than the whole portfolio ZIP as a repository file.

Official guidance: [Adding files to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository) and [File size limits](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github).

## Public copies and original sources

The report and drawing PDFs retain team attribution, source references, university ownership notices, and educational markings. Unnecessary student identifiers and PDF author metadata have been removed from the public copies. The full report retains its electrical-design chapters; separate KiCad source files are not included.

The original source archive and PDFs are preserved separately. Native CAD metadata is retained, as explained in cad/README.md.
