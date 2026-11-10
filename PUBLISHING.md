# Publishing the documentation

The documentation folder contains the illustrated README, original-resolution images, short technical notes, topic PDFs, and full public-copy team report. Separate KiCad project files are not included.

## Documentation upload

Upload the contents of this folder to the repository root. Keep the directory structure so relative links continue to work. A suitable commit message is:

Add SunnyPro project documentation and assembly drawings

## Native CAD

The companion original CAD archive is separate because it is large and retains the original file metadata and revisions. The native drawing exceeds GitHub's normal 100 MiB per-file Git limit.

Before publishing native CAD, review its metadata and dependencies in SolidWorks. Use a GitHub release asset or Git LFS for the large source files; do not add the companion archive through a normal Git commit. After uploading a release asset, add its real download URL to cad/README.md.

Official guidance: [About large files on GitHub](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github) and [Git Large File Storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage).

## Public-copy handling

The report and drawing retain team attribution, university ownership notices, source references, and educational-use markings. Student identifiers and unnecessary PDF author metadata have been removed from the public copies.

The original documents are preserved separately from this publication folder. The complete team report is included without removing its original electrical-design chapters.
