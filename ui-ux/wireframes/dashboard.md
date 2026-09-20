# Dashboard — SCR-UI-01

## Layout structure

```
+------------------------------------------+
| Top bar                                  |
| Logo | Search projects... | [New Project]|
+------------------------------------------+
|                                          |
|  Projects                                |
|  +------------------------------------+  |
|  | Project A  [Draft]  2 trace gaps  |  |
|  | Project B  [Ready]  0 trace gaps  |  |
|  | Project C  [Blocked] 5 trace gaps |  |
|  +------------------------------------+  |
|                                          |
+------------------------------------------+
```

## Sections

### Top bar
- Logo TraceSpec (kiri)
- Search bar (tengah)
- Primary CTA "New Project" (kanan)

### Projects list
- Card per project:
  - Name (clickable → Spec Workspace)
  - Status badge (Draft/Ready/Approved/Blocked)
  - Last updated
  - Trace gap count (warning icon + number)

## Interactions

- Click project name → navigate to Spec Workspace.
- Click "New Project" → navigate to New Project screen.
- Search: filter by project name.

## States

### Default
- Project list terisi.
- Search berfungsi.

### Empty
- Teks: "Belum ada proyek."
- Subtext: "Mulai dengan membuat proyek pertama Anda."
- CTA besar: "New Project".

### Loading
- Skeleton card untuk setiap project.
- Search disabled.
