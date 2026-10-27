# AdCodicem.Pdf.Corpus

Verbatim copies of third-party PDF documents that [AdCodicem.Pdf](https://github.com/AdCodicem/AdCodicem.Pdf)'s
test suite uses, kept so that a publisher's outage does not take them out of the nightly tests
([ADR 51](https://github.com/AdCodicem/AdCodicem.Pdf/blob/main/docs/adr/0051-the-project-keeps-a-copy-of-what-a-license-lets-it-copy.md)).

**Each file is under its own license, named below and in [`REUSE.toml`](REUSE.toml), with its texts in
[`LICENSES/`](LICENSES).** This repository grants no license of its own over them, and AdCodicem.Pdf's MIT license
does not reach them.

## Rules

- **Byte-identical.** Every file is the publisher's, unmodified, pinned by the SHA-256 and the size that
  AdCodicem.Pdf's [`tests/corpus/manifest.json`](https://github.com/AdCodicem/AdCodicem.Pdf/blob/main/tests/corpus/manifest.json)
  records for it. Nothing derived from a document — a damaged or repaired variant, a rendering — is ever committed
  here.
- **Nothing enters without an entry in that manifest**, whose `source.copy` records the review of the license, read
  again for that very file, that allowed the copy, and whose `source.publisher` keeps the publisher's URL.
- **The manifest pins a commit of this repository, never a branch**, so a file is never changed in place: a new
  version is a new document.
- **A file over 100 MB** is an asset of an immutable release rather than a file in git.
- A document found not to be covered by its license is removed, its history included, and returns to its
  publisher. To raise one, open an issue in AdCodicem.Pdf.
- **Nothing here is offered for sale or for any fee.** Some files — the Government of Canada's forms under `canada/` —
  may be reproduced for public non-commercial purposes only: they are unmodified copies, not official versions,
  their presence here implies no affiliation with or endorsement by the Government of Canada, and they may not be
  sold or redistributed commercially without the permission of the institution that published them
  ([`LICENSES/LicenseRef-canada-crown-copyright-non-commercial.txt`](LICENSES/LicenseRef-canada-crown-copyright-non-commercial.txt)).

## The documents (17 files, 104 documents)

| File | License | Attribution | Publisher | Where |
|---|---|---|---|---|
| `canada/livecycle-es10-ircc-imm1344-certified-dynamic-xfa.pdf` | LicenseRef-canada-crown-copyright-non-commercial | © His Majesty the King in right of Canada, represented by Immigration, Refugees and Citizenship Canada: "IMM 1344 (06-2019) E: Application to Sponsor, Sponsorship Agreement and Undertaking"; a copy of the version available at https://www.canada.ca/content/dam/ircc/migration/ircc/english/pdf/kits/forms/imm1344e.pdf, as the Internet Archive captured it on 2020-11-11 | https://web.archive.org/web/20201111224144id_/https://www.canada.ca/content/dam/ircc/migration/ircc/english/pdf/kits/forms/imm1344e.pdf | this tree |
| `canada/livecycle-es9-cfia-fish-export-license-dynamic-xfa.pdf` | LicenseRef-canada-crown-copyright-non-commercial | © His Majesty the King in right of Canada, represented by the Canadian Food Inspection Agency: "CFIA / ACIA 5704 (2013/01): Application for a Fish Export Licence"; a copy of the version available on the CFIA website at https://inspection.canada.ca/DAM/DAM-food-aliments/STAGING/text-texte/c5704_re_1357758804123_eng.pdf, as the Internet Archive captured it on 2021-06-09 | https://web.archive.org/web/20210609130056id_/https://inspection.canada.ca/DAM/DAM-food-aliments/STAGING/text-texte/c5704_re_1357758804123_eng.pdf | this tree |
| `govinfo/us-code-2023-title42.pdf` | LicenseRef-us-government-work | Office of the Law Revision Counsel, U.S. House of Representatives, "United States Code, 2023 Edition, Title 42 - The Public Health and Welfare", published by the U.S. Government Publishing Office, https://www.govinfo.gov/app/details/USCODE-2023-title42 | https://www.govinfo.gov/content/pkg/USCODE-2023-title42/pdf/USCODE-2023-title42.pdf | this tree |
| `ipres2017/radar-10.22000-53-v1.tar` | CC-BY-SA-4.0 | Michelle Lindlar (TIB), Yvonne Tunnat (ZBW) and Carl Wilson (OPF), "Synthetic PDF Testset for File Format Validation", RADAR, 2017, doi:10.22000/53, https://doi.org/10.22000/53, CC BY-SA 4.0 | https://www.radar-service.eu/radar-backend/archives/JtlOdwQquZWDqQdq/versions/1/content | this tree |
| `ocrmypdf/epson-scan-indirect-rotate.pdf` | CC-BY-SA-3.0 | Contributors to the English Wikipedia article "Optical character recognition" (revision of 2016-09-14, history: https://en.wikipedia.org/w/index.php?title=Optical_character_recognition&action=history); printed and scanned by James R. Barlow as OCRmyPDF test resource "tests/resources/epson.pdf", https://github.com/ocrmypdf/OCRmyPDF, CC BY-SA 3.0 | https://raw.githubusercontent.com/ocrmypdf/OCRmyPDF/e59d7627dd7f4e17d117b24f1c636dc37789fa93/tests/resources/epson.pdf | this tree |
| `ocrmypdf/kodak-capture-scan-broken-outline.pdf` | CC-BY-SA-4.0 | James R. Barlow (C) 2025, OCRmyPDF test resource "tests/resources/kcs.pdf", https://github.com/ocrmypdf/OCRmyPDF, CC BY-SA 4.0 | https://raw.githubusercontent.com/ocrmypdf/OCRmyPDF/e59d7627dd7f4e17d117b24f1c636dc37789fa93/tests/resources/kcs.pdf | this tree |
| `ocrmypdf/photoshop-cc2015-pdfx3-cmyk.pdf` | CC-BY-SA-4.0 | James R. Barlow (C) 2025, OCRmyPDF test resource "tests/resources/cmyk.pdf", https://github.com/ocrmypdf/OCRmyPDF, CC BY-SA 4.0 | https://raw.githubusercontent.com/ocrmypdf/OCRmyPDF/e59d7627dd7f4e17d117b24f1c636dc37789fa93/tests/resources/cmyk.pdf | this tree |
| `ocrmypdf/tiff2pdf-35000px-ccitt-image.pdf` | CC-BY-SA-4.0 | James R. Barlow (C) 2025, OCRmyPDF test resource "tests/resources/hugemono.pdf", https://github.com/ocrmypdf/OCRmyPDF, CC BY-SA 4.0 | https://raw.githubusercontent.com/ocrmypdf/OCRmyPDF/e59d7627dd7f4e17d117b24f1c636dc37789fa93/tests/resources/hugemono.pdf | this tree |
| `opf-format-corpus/pdfmaker81-word-va-kernel-systems-guide.pdf` | LicenseRef-us-government-work | Department of Veterans Affairs, Office of Information & Technology, "Kernel Systems Management Guide, Version 8.0" (VistA, revised June 2008), via GovDocs1 / the OPF format-corpus, https://github.com/openpreserve/format-corpus | https://raw.githubusercontent.com/openpreserve/format-corpus/366f068cec399d0cdfd61fa473de3ab6dc858098/govdocs1-error-pdfs/error_set_1/499039.pdf | this tree |
| `opf-format-corpus/pdfmaker9-word-distiller-embedded-avi.pdf` | CC0-1.0 | Johan van der Knijff (Koninklijke Bibliotheek), "embedded_video_avi.pdf", Open Preservation Foundation format-corpus, https://github.com/openpreserve/format-corpus/tree/master/pdfCabinetOfHorrors, CC0 1.0 | https://raw.githubusercontent.com/openpreserve/format-corpus/366f068cec399d0cdfd61fa473de3ab6dc858098/pdfCabinetOfHorrors/embedded_video_avi.pdf | this tree |
| `pdf20examples/handwritten-pdf20-utf8-strings.pdf` | CC-BY-SA-4.0 | PDF Association (Peter Wyatt), "pdf20-utf8-test.pdf", https://github.com/pdf-association/pdf20examples, CC BY-SA 4.0 | https://raw.githubusercontent.com/pdf-association/pdf20examples/c20f2c17bfcc4baab7cfe62e70fae64caf14d5fa/pdf20-utf8-test.pdf | this tree |
| `py-pdf-sample-files/google-docs-document.pdf` | CC-BY-SA-4.0 AND Apache-2.0 | Martin Thoma and the py-pdf/sample-files contributors, "google-doc-document.pdf" (011-google-doc-document), https://github.com/py-pdf/sample-files, CC BY-SA 4.0; snake emoji from Google's Noto Emoji, Copyright Google Inc., Apache-2.0 | https://raw.githubusercontent.com/py-pdf/sample-files/02b8203bf416db3dbdb03438bc8278dfcb0555f3/011-google-doc-document/google-doc-document.pdf | this tree |
| `py-pdf-sample-files/pdftex-outline.pdf` | CC-BY-SA-4.0 | Martin Thoma and the py-pdf/sample-files contributors, "pdflatex-outline.pdf" (006-pdflatex-outline), https://github.com/py-pdf/sample-files, CC BY-SA 4.0 | https://raw.githubusercontent.com/py-pdf/sample-files/02b8203bf416db3dbdb03438bc8278dfcb0555f3/006-pdflatex-outline/pdflatex-outline.pdf | this tree |
| `py-pdf-sample-files/weasyprint-arabic.pdf` | CC-BY-SA-4.0 | Daniel Kahn Gillmor (dkg) and the py-pdf/sample-files contributors, "habibi.pdf" (015-arabic), https://github.com/py-pdf/sample-files, CC BY-SA 4.0 | https://raw.githubusercontent.com/py-pdf/sample-files/02b8203bf416db3dbdb03438bc8278dfcb0555f3/015-arabic/habibi.pdf | this tree |
| `py-pdf-sample-files/wkhtmltopdf-qt5-html-page.pdf` | CC-BY-SA-4.0 | Martin Thoma and the py-pdf/sample-files contributors, "pdfkit.pdf" (022-pdfkit), https://github.com/py-pdf/sample-files, CC BY-SA 4.0 | https://raw.githubusercontent.com/py-pdf/sample-files/02b8203bf416db3dbdb03438bc8278dfcb0555f3/022-pdfkit/pdfkit.pdf | this tree |
| `usgs/omnipage-usgs-professional-paper-1-1902.pdf` | LicenseRef-us-government-work | Alfred Hulse Brooks, U.S. Geological Survey, "Preliminary report on the Ketchikan mining district, Alaska", Professional Paper 1, Government Printing Office, 1902, https://pubs.usgs.gov/publication/pp1 | https://pubs.usgs.gov/pp/0001/report.pdf | release asset |
| `usgs/us-topo-washington-west-2023.pdf` | LicenseRef-us-government-work | U.S. Geological Survey, "Washington West, DC-MD-VA US Topo 7.5-minute quadrangle, 2023", https://www.usgs.gov/programs/national-geospatial-program/us-topo-maps-america | https://prd-tnm.s3.amazonaws.com/StagedProducts/Maps/USTopo/PDF/DC/DC_Washington_West_20230612_TM_geo.pdf | this tree |
