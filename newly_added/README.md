# Newly Added Product Documents

Place unsynchronized original UROVO product documents in this directory, then explicitly ask an Agent with repository write access to process this inbox by following `../SYNC_PROMPT.md`. This README is only the inbox entry guide; `../SYNC_PROMPT.md` is the complete execution contract.

Rules:

- Normally add original PDF/PPTX/DOCX/XLSX, PNG/JPG/WebP, or equivalent documents; single-product and multi-product inputs are both accepted.
- A standalone Markdown input is also allowed when the user explicitly identifies it as personally authored or approves it as canonical knowledge. Keep that Markdown unchanged as the one-file canonical source; do not create a duplicate companion.
- A Markdown correction to an existing companion is allowed only when supported by the retained original.
- Pure-image files, scanned pages, and image-dominant slides must be visually inspected in full. The synchronized Markdown must transcribe their readable text, tables, labels, and meaningful visual content; image links, placeholders, or “see original” references are not substitutes for visual recognition.
- If visual capability is unavailable, any page or image cannot be inspected, or extraction cannot be verified, leave the input here and report the blocker. Do not claim success or remove the input.
- Normal product Q&A ignores this directory.
- Successfully synchronized files are removed from this inbox.
- Ambiguous or failed inputs remain here for review.
- This README is not an input document.
