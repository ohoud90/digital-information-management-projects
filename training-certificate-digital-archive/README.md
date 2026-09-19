# Training Certificate Digital Archive

## Overview | نبذة

This case study documents a completed digital-archiving workflow for approximately **385 scanned training certificates across four programs**. The public version describes the method using synthetic examples and contains no original certificates or personal data.

توثق دراسة الحالة مسار عمل منجزًا لأرشفة نحو **385 شهادة تدريب ممسوحة ضوئيًا موزعة على أربعة برامج**. تستخدم النسخة العامة أمثلة اصطناعية ولا تتضمن الشهادات الأصلية أو أي بيانات شخصية.

## Business Need | الحاجة

Transform scanned, difficult-to-search PDF certificates into a controlled index with consistent filenames, traceable metadata, retrieval links, and repeatable quality checks.

تحويل شهادات PDF الممسوحة ضوئيًا وصعبة البحث إلى فهرس منضبط يحتوي على أسماء ملفات موحدة وبيانات وصفية قابلة للتتبع وروابط استرجاع وفحوص جودة قابلة للتكرار.

## Workflow | سير العمل

1. Inventory source PDF batches.
2. Structure metadata in Excel.
3. Split multi-page PDF files.
4. Match sequential records to certificate pages.
5. Generate standardized filenames.
6. Upload controlled copies and create retrieval links.
7. Validate filename, record, and link coverage.
8. Log exceptions for manual review.

## Tools | الأدوات

- Microsoft Excel for metadata and reconciliation.
- Python for PDF separation, renaming, and automated checks.
- Google Apps Script / JavaScript for link and sheet automation.
- Google Drive for controlled retrieval links.
- PDF tools for visual inspection and exception handling.

## Challenges Addressed | التحديات

- Image-based PDFs and limited text extraction.
- Arabic UTF-8 filename handling.
- Sequential metadata matching.
- Duplicate output prevention.
- Shifting identifier columns.
- Smart-skip logic and combined automated/manual quality assurance.

## Outcome | النتيجة

A structured and searchable certificate index with consistent naming, improved retrieval, documented exceptions, and repeatable quality-control steps.

## Public Assets | الملفات العامة

- `sample-data/certificate_index_sample.csv`: synthetic metadata example.
- Demonstration scripts will be added only after removing all environment-specific paths and identifiers.

