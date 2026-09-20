# Screen Inventory — TraceSpec

| ID | Screen | User goal | Primary action | States | Requirement |
|---|---|---|---|---|---|
| SCR-01 | Idea Canvas | Memasukkan ide dan konteks | Analyze idea | default, validation, loading, error | FR-01 |
| SCR-02 | MVP Challenge | Menyetujui/ubah scope MVP | Lock MVP | default, warning, approved | FR-02 |
| SCR-03 | Spec Workspace | Meninjau PRD dan artefak | Generate/Revise | default, trace-gap, loading | FR-03 |
| SCR-04 | Build Packet | Meninjau task dan handoff agent | Generate packet | default, ready, blocked | FR-04 |
| SCR-05 | Change Impact | Memahami dampak revisi | Approve revision | default, high-risk, approved | FR-05 |

Setiap screen wajib memiliki empty, loading, error, responsive behavior, dan accessibility state dalam implementasi UX detail.
