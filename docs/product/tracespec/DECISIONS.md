# Decision Records — TraceSpec

## ADR-01 — Markdown and GitHub as MVP source of truth

**Decision:** Simpan artefak dalam Markdown yang versioned di GitHub.

**Rationale:** Transparan, mudah ditinjau, portable ke coding agent, dan tidak memerlukan database graph pada MVP.

**Alternative rejected:** Membuat database/proprietary visual workspace sejak awal.

## ADR-02 — Traceability through stable IDs

**Decision:** Gunakan ID seperti P-XX, FR-XX, FLOW-XX, SCR-XX, TASK-XX, dan TEST-XX.

**Rationale:** Impact analysis dapat dilakukan secara deterministik dan dokumen dapat ditautkan tanpa bergantung pada judul yang berubah.

## ADR-03 — Approval before GitHub writes

**Decision:** Semua create/update/push harus dipreview dan disetujui pengguna.

**Rationale:** Mencegah artefak yang tidak akurat masuk ke source of truth.
