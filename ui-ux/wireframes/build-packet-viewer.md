# Build Packet Viewer — SCR-UI-04

## Layout structure

```
+-------------------------------------------------------------+
| Top bar                                                     |
| [Back] Build Packets | Milestone 01 — Foundation | [Export] |
+-------------------------------------------------------------+
|                                                             |
| Header                                                      |
| Name, Version (v0.1), Status (Ready/Blocked)                |
|                                                             |
+-------------------------------------------------------------+
| Content                                                     |
|                                                             |
| Objective                                                   |
| [Text paragraf]                                             |
|                                                             |
| Scope In / Scope Out                                        |
| [Two columns]                                               |
|                                                             |
| Linked Requirements                                         |
| [Chips: FR-01, FR-03]                                       |
|                                                             |
| Tasks                                                       |
| - TASK-01: ... [Done]                                       |
| - TASK-02: ... [In progress]                                |
| - TASK-03: ... [Todo]                                       |
|                                                             |
| Acceptance Tests                                            |
| - TEST-01: ...                                              |
| - TEST-03: ...                                              |
|                                                             |
| Agent Prompt                                                |
| +--------------------------+                                |
| | agent-prompt.md content  | [Copy]                         |
| +--------------------------+                                |
|                                                             |
| Actions                                                     |
| [Copy Prompt] [Export] [Commit to GitHub]                   |
|                                                             |
+-------------------------------------------------------------+
```

## Sections

### Header
- Milestone name.
- Version badge.
- Status badge (Ready/Blocked).

### Objective
- Paragraf singkat tentang tujuan milestone.

### Scope In / Out
- Two columns:
  - Scope In: apa yang dikerjakan.
  - Scope Out: apa yang tidak dikerjakan.

### Linked Requirements
- Chips ID requirement yang terkait.

### Tasks
- List task dengan status (Todo, In progress, Done).

### Acceptance Tests
- List test scenarios.

### Agent Prompt
- Code block dengan isi `agent-prompt.md`.
- Button "Copy" untuk clipboard.

### Actions
- Copy Prompt.
- Export (download ZIP/JSON).
- Commit to GitHub (bila terintegrasi).

## States

### Ready
- Semua section terisi.
- Actions aktif.

### Blocked
- Warning: "Dependencies belum terpenuhi."
- Actions disabled atau sebagian saja.
