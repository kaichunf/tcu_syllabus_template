# TCU syllabus — pdfLaTeX template

This is an editable template transcribed from `COSC_50513_Machine_Learning_Syllabus_v2.docx`, using the supplied PDF as an additional visual reference. It uses **pdfLaTeX** (not XeLaTeX), Arial-compatible **Arimo**, 12pt type, U.S. Letter, 1-inch margins, purple headings (`#4D1979`), color tables, and a running copyright footer.

## Build

```bash
latexmk tcu-syllabus.tex
```

The exact `.latexmkrc` supplied by the user directs **every** generated file, including the PDF, to `.latexmk/`.

Output: `.latexmk/tcu-syllabus.pdf`.

To rebuild from scratch:

```bash
latexmk -C tcu-syllabus.tex
latexmk tcu-syllabus.tex
```

## Customize

- `course-info.tex`: course/instructor field values.
- `tcu-syllabus.tex`: front page layout and placeholder logo/QR images.
- `sections/course-description.tex`: catalog description, outcomes, SLO mapping.
- `sections/course-requirements.tex`: assignment and grading tables.
- `sections/course-policies.tex`: academic conduct, late work, attendance, AI alternatives.
- `sections/course-schedule.tex`: 16-week course schedule.
- `tcu-syllabus.sty`: styling, margins, footer, colors, table definitions.

### Important source-version discrepancy

The attached PDF is **not a PDF conversion of the attached DOCX revision**. The PDF includes a table of contents and 3-column schedule; the DOCX includes an SLO assessment table, revised grading cutoffs, and a **4-column** course schedule. This project follows the **DOCX content and section order**. Logo and QR-code images are placeholders.

The DOCX contains **all three alternative AI policy statements (A/B/C)** rather than a chosen policy; review and select the correct option for use in an actual course. Other course-specific dates and policies should also be reviewed each semester.

### Fidelity note

This is a reproducible, fully editable pdfLaTeX rendering, not a pixel-identical reproduction of Word. Arial is substituted with Arimo to keep pdflatex compatibility; spacing, hyphenation, and page breaks can differ from Word. Tweak style dimensions in `tcu-syllabus.sty` if exact pagination becomes important.
