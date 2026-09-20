# Spec Workspace — SCR-UI-03

## Layout structure

```
+-------------------------------------------------------------+
| Top bar                                                     |
| [Back] Project Name | [Status] | [Generate Packet] | [...]  |
+-------------------------------------------------------------+
| Outline | PRD Content                  | Traceability Panel |
|         |                              |                    |
| Problem | # Product Requirements Doc   | Linked Artifacts   |
| Goals   |                              |                    |
| Reqs    | ## Problem                   | P-01  [problem]    |
| Flows   |                              | G-01  [goal]       |
| Screens | Text paragraf...             | FR-01 [requirement]|
| Tasks   |                              | FLOW-01 [flow]     |
| Tests   | ### P-01 — Problem name      | SCR-01 [screen]    |
|         |                              | TASK-01 [task]     |
|         | [TRACE GAP] Warning          | TEST-01 [test]     |
|         |                              |                    |
+---------+------------------------------+--------------------+
```

## Sections

### Top bar
- Back button (kiri)
- Project name
- Status badge (Draft/Ready/Approved)
- Primary action: "Generate Build Packet"
- Menu dropdown (settings, export, dll.)

### Left: Document outline
- Daftar section PRD:
  - Problem
  - Goals
  - Requirements
  - Flows
  - Screens
  - Tasks
  - Tests
- Click section → scroll ke bagian terkait.

### Center: PRD content
- Render Markdown PRD.
- Heading jelas (H1, H2, H3).
- Requirement blocks dengan ID (FR-01, FR-02, dst.).
- Trace gap warning inline bila ada missing links.

### Right: Traceability panel
- Section: "Linked Artifacts"
- Chips ID:
  - P-01 [problem]
  - G-01 [goal]
  - FR-01 [requirement]
  - FLOW-01 [flow]
  - SCR-01 [screen]
  - TASK-01 [task]
  - TEST-01 [test]
- Click chip → navigate ke artifact terkait (bila ada halaman terpisah).

## Interactions

- Click outline section → scroll smooth ke section.
- Click chip ID → open detail artifact / highlight di dokumen.
- Click "Generate Build Packet" → navigate ke Build Packet Viewer.

## States

### Default
- PRD lengkap.
- Traceability panel terisi.

### Trace-gap
- Warning box: "[TRACE GAP] FR-03 belum memiliki test."
- Visual highlight pada requirement terkait.

### Loading
- Skeleton untuk outline dan content.
- Traceability panel disabled.
