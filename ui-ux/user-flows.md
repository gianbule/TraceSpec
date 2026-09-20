# User Flows — TraceSpec UI

## FLOW-UI-01 — Create new project

**Actor:** Solo builder / founder

**Goal:** Membuat proyek baru dari ide.

**Steps:**
1. User masuk ke Dashboard.
2. Klik "New Project".
3. Masukkan nama proyek dan ide singkat.
4. Sistem membuat project skeleton di GitHub.
5. User diarahkan ke Spec Workspace.

**States:**
- Default: daftar proyek ada.
- Empty: belum ada proyek, CTA "New Project" menonjol.
- Loading: saat membuat proyek.
- Success: redirect ke Spec Workspace.

---

## FLOW-UI-02 — Explore PRD dan traceability

**Actor:** Product owner / AI-first developer

**Goal:** Membaca PRD dan memahami hubungan antar artefak.

**Steps:**
1. User membuka project dari Dashboard.
2. Lihat outline dokumen di kiri.
3. Klik requirement (mis. FR-03).
4. Panel kanan menampilkan linked artifacts: flows, screens, tasks, tests.
5. User dapat klik chip ID untuk navigasi cepat.

**States:**
- Default: PRD lengkap.
- Trace-gap: ada warning visual.
- Loading: saat memuat dokumen.

---

## FLOW-UI-03 — Generate build packet

**Actor:** AI-first developer / solo builder

**Goal:** Mendapatkan prompt implementasi siap pakai.

**Steps:**
1. User membuka tab "Build Packets".
2. Pilih milestone.
3. Lihat scope, tasks, tests, dan agent prompt.
4. Klik "Copy Prompt" atau "Export".
5. Opsional: trigger GitHub commit untuk versi baru.

**States:**
- Ready: packet lengkap.
- Blocked: dependency belum terpenuhi.
- Loading: saat generate/export.

---

## FLOW-UI-04 — Revise requirement

**Actor:** Product owner

**Goal:** Mengubah requirement dengan aman.

**Steps:**
1. User mengedit requirement di PRD.
2. Klik "Analyze Impact".
3. Sistem menampilkan change impact report.
4. User approve/defer/reject.
5. Sistem update dokumen terkait dan changelog.

**States:**
- Default: mode baca.
- Edit: mode edit requirement.
- High-risk: impact besar.
- Approved: revisi diterapkan.
