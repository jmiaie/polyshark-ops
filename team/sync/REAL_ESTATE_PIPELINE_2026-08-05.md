# Real Estate Pipeline — Deployed 2026-08-05

## Status: LIVE

**Location:** `/home/ubuntu/.openclaw/workspace/repos/real-estate-pipeline/`

## Structure
- `input/` — Drop docs here (CSV, XLSX, DOCX, PDF)
- `processed/` — Clean markdown output
- `output/extracted/` — Structured JSON data
- `scripts/process_docs.py` — Main processor with smart extraction

## anydoc Integration
- **anydoc version:** 0.1.4
- **Installed:** Globally via npm (`/usr/bin/anydoc`)
- **Repo:** `/home/ubuntu/.openclaw/workspace/repos/anydoc/`
- **Purpose:** Convert Office docs (Word, Excel, PowerPoint, PDF) → clean Markdown

## Smart Extraction
Auto-detects doc type and extracts relevant fields:
- **legal_letter** — recipient, date, account/re line
- **property_disclosure** — owner, address, sqft, year built, lot size, HOA, defects
- **foreclosure_notice** — case no, address, parcel ID, sale date
- **county_export** — table extraction (address, owner, value, year, zoning, etc.)

## Test Results (5/5 converted)
1. County export CSV → 3 properties with full fields
2. Property records CSV → 5 properties
3. Property records XLSX → 3 properties
4. Debt validation letter DOCX → Legal letter detected
5. Property disclosure PDF → Full property data extracted

## Usage
```bash
cd /home/ubuntu/.openclaw/workspace/repos/real-estate-pipeline
python3 scripts/process_docs.py
```

## Next Steps
- Drop real county exports, property PDFs, lead files into `input/`
- Run processor to convert and extract
- Structured data ready for AI analysis, lead scoring, outreach

## Notes
- No OCR fallback tested yet (scanned PDFs / image-heavy docs)
- All test files were text-based — no OCR needed
- Pipeline reduces manual data entry from county exports (saves 15-30 min per batch)
