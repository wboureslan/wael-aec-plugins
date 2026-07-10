---
name: submittal
description: Draft material and shop-drawing submittals and their transmittals for consultant/engineer approval, formatted to the project specification. Trigger with "prepare a submittal", "material submittal for", "material approval request", "MAR for", "shop drawing submittal", "prepare a transmittal", or when the user needs to get a product, sample, or shop drawing approved before use on site. Tuned for building, fit-out, and general-contracting projects.
---

# Submittal / Material Approval

Prepare a submittal package that gets a material, product, sample, or shop drawing approved by the consultant/engineer. A good submittal maps the proposed item to every relevant specification requirement so the reviewer can approve it in one pass.

## Step 1 — Identify the submittal type

- **Material / Product Approval (MAR / MAS)** — approve a specific product against a spec section.
- **Sample submittal** — physical samples for colour/finish/quality approval.
- **Shop / working drawing submittal** — fabrication or installation drawings.
- **Prequalification / vendor approval** — approve a supplier or subcontractor.

Ask which type if unclear, and identify the governing **specification section** and the **project**.

## Step 2 — Gather content

- **Item** — product name, manufacturer, model/reference, country of origin.
- **Governing spec section & clauses** — read the attached spec; extract every mandatory requirement (properties, ratings, standards, samples required, warranty).
- **Supporting documents the reviewer expects**: technical datasheet, test certificates / compliance to standards, manufacturer catalogue, samples list, warranty, method of installation reference, and any local authority / civil-defence approval where required.
- **Drawings/locations** where the item will be used.

If the user attaches a datasheet or spec, read them and pull values directly.

## Step 3 — Build a compliance statement

The heart of a strong submittal is a clause-by-clause compliance statement: list each spec requirement, the proposed item's corresponding value/evidence, and a Comply / Comment column. This mirrors the reviewer's checklist and speeds approval. Reuse the matrix format from the `rfi-spec-compliance` skill's compliance checklist if that skill is available.

Mark honestly: where the datasheet does not evidence a requirement, note it and flag what certificate is needed — do not overstate compliance.

## Step 4 — Assemble the package & transmittal

Assemble in the order a reviewer reads:

1. **Submittal cover / register entry** — submittal number placeholder, project, spec section, revision, date, status (New / Resubmission).
2. **Transmittal letter** — from contractor to consultant, listing enclosed documents and the action requested (Approve / Approve as noted / Revise & resubmit).
3. **Compliance statement** — the clause-by-clause matrix.
4. **Technical datasheets & certificates** — listed as attachments/placeholders.
5. **Samples schedule** — where physical samples accompany the submittal.
6. **Consultant action block** — status codes (A — Approved, B — Approved as noted, C — Revise & resubmit, D — Rejected) with reviewer name/date.

See `references/submittal-package.md` for the full structure, status codes, and a worked example.

## Step 5 — Deliverable

Default to a Word document for the transmittal + compliance statement (use the `docx` skill), formatted for transmittal to the consultant; offer a PDF export for issuing, and merge attachments if the user provides them (use the `pdf` skill to combine into one submittal PDF). For a submittal register or a multi-item log, use a spreadsheet (`xlsx` skill).

Leave placeholders for submittal numbers, dates, and names — do not invent them. Do not fabricate test-certificate values or approvals.
