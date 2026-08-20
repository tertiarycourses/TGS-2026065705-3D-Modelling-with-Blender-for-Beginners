# Courseware QA Report — v11.0

Course: **3D Modelling with Blender for Beginners**

Course code: **TGS-2022015368**

Audit date: **20 August 2026**

## Overall verdict

**PASS — ready for controlled Drive, LMS-TMS and public GitHub publication.**

## A. PowerPoint

**PASS**

- 136 slides; white-theme, concept-led delivery.
- General trainer profile and named Dr Alfred Ang profile are separate visual slides.
- Course-material access, assessment flow and final attendance are visual flows.
- Cover has one version label: v11.0.
- Final sequence is Assessment Reminder → Assessment Flow → Digital Attendance → Thank You.
- Detailed procedures are not duplicated in the slides.
- 26 embedded media assets include five course-specific generated visuals and 20 distinct Blender visual references retained from the legacy deck.
- All 136 slides were rendered and reviewed through 12 contact sheets. Fresh-eyes re-audit found no clipping, overlap, broken images or illegible primary text.
- The course is not a certification/exam-preparation programme, so a practice-exam slide is not applicable.

## B. Assessment

**PASS**

| Criterion | Instrument | Coverage |
|---|---|---|
| K1–K9 | WA (SAQ) | 9 open-ended questions; one printed K code per question |
| A1–A2 | PP Task 1 | Labs 1–2; creative brief, polygon budget and blockout |
| A3–A4 | PP Task 2 | Labs 3–4; modelling, sculpting, topology review and refinement |
| A5–A6 | PP Task 3 | Labs 5–6; materials, rigging, animation and presentation |
| A7–A8 | PP Task 4 | Labs 7–8; feedback, lighting, optimisation, export and verification |

- Original instrument types preserved: WA + PP.
- Original counts preserved: 9 WA questions + 4 PP tasks.
- Original live-paper timings preserved: 60-minute WA + 90-minute PP.
- Four DOCX files generated: two candidate papers and two trainer-only answer keys.
- Candidate papers use the required cover → trainee/instructions/grading → scenario/questions order.
- All assessment pages were rendered; no clipping, overlap or broken response areas were found.

## C. Lesson Plan

**PASS**

- WSQ cover, version-control record and populated contents index included.
- Two-day schedule totals 16 instructional/assessment hours excluding lunch.
- Slide ranges were regenerated from `slide_map.json` and checked against the 136-slide deck.
- PDF render: 7 pages; no clipping or overlap.

## D. Learner Guide

**PASS**

- WSQ cover, version-control record and populated contents index included.
- 21 pages with detailed 12-step procedures for each of the eight labs.
- Exact learner-facing lab folder names are printed.
- DOCX and PDF were regenerated from the same source module.
- A separate Learner Guide Markdown mirror is intentionally not distributed under the current learner-guide ownership rule; detailed lab Markdown/PDF pairs remain in each lab folder.

## E. Labs and alignment

**PASS with declared compatibility note**

- Eight self-contained folders.
- Every lab contains `STARTER.blend`, `EXAMPLE.blend`, `README.md/.pdf`, `INSTRUCTIONS.md/.pdf`, `CHECKLIST.md/.pdf` and `Example-Presentation.pptx`.
- Each lab procedure contains 12 numbered steps plus acceptance and evidence checks.
- 25 learner-facing lab Markdown files have same-basename PDF parity.
- All 16 Blender files have valid `BLENDER-v291` headers and stable SHA-256 checksums.
- The supplied sample files originate from Blender 2.91. The lab instructions require learners to open a copy in current Blender and use Save As before editing. Blender is not installed on this build machine, so interactive opening/rendering was not claimed as tested.

## F. Files and distribution

**PASS**

- Current PPTX/PDF, LG DOCX/PDF and LP DOCX/PDF exist in `courseware/`.
- All PPTX/DOCX packages passed ZIP/OOXML integrity checks; all PDFs passed `pdfinfo` validation.
- `assessment/`, `reference/`, `.env`, build tooling and QA renders are Git-ignored.
- Answer keys are restricted to Google Drive and are excluded from LMS-TMS and GitHub publication.
- Google Drive dry-run and controlled upload completed against the supplied folder. Post-write readback confirmed eight lab folders, public candidate papers and trainer-only answer keys in a limited-access folder.

## Command compatibility

- `/wsq-setup`, `/courseware-gen`, `/courseware-qa`, `/assessment-gen` and `/gdrive-push` equivalents were executed from the installed project command set.
- The requested spelling `/assessemnt-gen` maps to the installed `/assessment-gen` command.
- No `/tms-push-qa` command exists in the installed command set; its available intent is covered by QA and Drive dry-run/post-write readback.
- `/tms-push` reached the LMS-TMS API but stopped safely at `401 Not authenticated`; no LMS-TMS write or readback is claimed.
