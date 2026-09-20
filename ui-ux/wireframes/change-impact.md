# Change Impact — SCR-UI-05

## Layout structure

```
+-------------------------------------------------------------+
| Top bar                                                     |
| [Back] Change Impact | Revision #3 | [Cancel] [Approve]     |
+-------------------------------------------------------------+
|                                                             |
| Change Request                                              |
| [Text box atau summary perubahan]                           |
|                                                             |
+-------------------------------------------------------------+
| Before / After                                              |
| +------------------+ +------------------+                   |
| | Before (v0.3)    | | After (v0.4)     |                   |
| | - Scope lama     | | + Scope baru     |                   |
| | - Feature A      | | - Feature A      |                   |
| |                  | | + Feature B      |                   |
| +------------------+ +------------------+                   |
+-------------------------------------------------------------+
| Affected Artifacts                                          |
|                                                             |
| PRD Sections                                                |
| - Problem, Requirements, Flows                              |
|                                                             |
| Requirements                                                |
| [FR-01] [FR-03] [FR-05]                                     |
|                                                             |
| Flows                                                       |
| [FLOW-01] [FLOW-03]                                         |
|                                                             |
| Screens                                                     |
| [SCR-01] [SCR-03] [SCR-05]                                  |
|                                                             |
| Tasks                                                       |
| [TASK-01] [TASK-03] [TASK-05]                               |
|                                                             |
| Tests                                                       |
| [TEST-01] [TEST-03]                                         |
|                                                             |
+-------------------------------------------------------------+
| Risks & Recommendation                                      |
| Risk level: [High/Medium/Low]                               |
| Version: v0.3 → v0.4                                        |
| Recommendation: Approve / Defer                             |
|                                                             |
+-------------------------------------------------------------+
| Actions                                                     |
| [Approve Revision] [Defer to Phase 2] [Reject]              |
|                                                             |
+-------------------------------------------------------------+
```

## Sections

### Change Request
- Summary perubahan yang diminta user.
- Bisa berupa teks bebas atau structured diff.

### Before / After
- Two panels:
  - Before: state sebelumnya.
  - After: state setelah perubahan.
- Highlight added/removed/changed items.

### Affected Artifacts
- Grouped by type:
  - PRD Sections
  - Requirements (chips)
  - Flows (chips)
  - Screens (chips)
  - Tasks (chips)
  - Tests (chips)

### Risks & Recommendation
- Risk level badge (High/Medium/Low).
- Version recommendation (v0.3 → v0.4).
- Short rationale.

### Actions
- Approve Revision → terapkan perubahan, update dokumen, commit.
- Defer to Phase 2 → tandai sebagai future consideration.
- Reject → batalkan perubahan.

## States

### Default
- Impact normal.
- Semua sections terisi.

### High-risk
- Warning banner: "Perubahan ini berdampak besar pada scope MVP."
- Risk level badge merah.
- Confirm dialog sebelum approve.

### Approved
- Success message: "Revisi diterapkan. Versi: v0.4."
- Redirect ke Spec Workspace atau Build Packet.
