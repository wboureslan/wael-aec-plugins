---
name: rfi-spec-compliance
description: Draft Requests for Information (RFIs) and check drawings, materials, or executed work against project specifications and codes for compliance. Trigger with "raise an RFI", "draft an RFI for", "RFI about", "check spec compliance", "does this comply with the spec", "compliance check against the specification", "review this against the spec/code", or when there is a drawing conflict, missing detail, ambiguity, or a proposed material/substitution that needs consultant clarification or a conformity check. Tuned for building, fit-out, and general-contracting projects.
---

# RFI & Spec Compliance

Two related jobs: (A) draft clear Requests for Information to the consultant/engineer, and (B) check something against the project specification and applicable codes and report compliance. Decide which the user needs — or do both (a compliance gap often becomes an RFI).

## A. Drafting an RFI

An RFI asks the design team to resolve an ambiguity, conflict, missing detail, or discrepancy — not to shift design liability. Keep it factual, specific, and answerable.

### Gather
- **Subject** — one line summarising the query.
- **Trigger** — drawing conflict, spec ambiguity, missing detail, site condition, or proposed alternative.
- **References** — drawing numbers/revisions, spec sections/clauses, and the exact location (grid, level, room).
- **Impact** — potential effect on programme, cost, or interfaces (state if time-sensitive and give a required-by date).
- **Contractor's proposal / suggested resolution** — where you have one, offer it (this speeds the response).

If drawings or specs are attached, read them and cite exact references rather than asking.

### Draft
Produce an RFI with: RFI number placeholder, project, date raised, from/to, subject, detailed question, references, contractor's proposed solution, cost/time impact flag, required-by date, and a response block for the consultant. See `references/rfi-template.md` for the full field list and a worked example.

Keep the question crisp and answerable with a yes/no or a specific instruction where possible. Attach or reference the relevant drawing extracts.

## B. Spec / code compliance check

Compare a subject (proposed material, shop drawing, sample, or executed work) against the governing specification and codes, and report conformity.

### Gather
- **Subject** — what is being checked (e.g. a proposed tile, a fire-rated door datasheet, a screed thickness).
- **Governing spec** — the relevant specification section/clauses. Read the attached spec; if missing, ask for the section.
- **Applicable codes/standards** — project spec often invokes BS/EN, ASTM, ACI, ISO, or local authority/civil-defence requirements. Note the region.

### Method
1. Extract the mandatory requirements from the spec clause(s): properties, ratings, tolerances, standards referenced, submittal requirements, and any "or approved equal" conditions.
2. Extract the corresponding attributes of the subject (from datasheet, drawing, or measured values).
3. Compare attribute-by-attribute. For each requirement, mark **Complies / Does not comply / Insufficient information**, with the evidence and the clause reference.
4. Summarise: overall verdict, non-conformities, and missing data needed to close out.
5. Where a gap is a genuine ambiguity in the design/spec, recommend raising an RFI (and offer to draft it).

Present the result as a compliance matrix (requirement | spec clause | subject value | verdict | note). See `references/compliance-checklist.md` for the matrix format and common requirement categories.

### Guardrails
Do not assert compliance beyond the evidence provided — if a datasheet omits a property, mark it "insufficient information," not "complies." Do not invent test values, ratings, or clause numbers. Flag anything requiring a specialist or third-party test certificate.

## Deliverable
For an RFI, default to a Word document (use the `docx` skill) formatted for transmittal; offer PDF. For a compliance check, a Word document or a spreadsheet matrix (use `xlsx`) both work — ask or default to Word with an embedded table for a single item, xlsx for many items. Leave placeholders for RFI numbers, dates, and names.
