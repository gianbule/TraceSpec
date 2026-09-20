# Screen Inventory — TraceSpec UI

## SCR-UI-01 — Dashboard

**User goal:** Lihat semua proyek dan status.

**Primary action:** New Project / Open Project.

**Key elements:**
- Project list (name, status, last updated, trace gaps).
- Search/filter bar.
- Primary CTA: "New Project".

**States:**
- Default: proyek ada.
- Empty: belum ada proyek.
- Loading: memuat daftar.

---

## SCR-UI-02 — New Project

**User goal:** Buat proyek baru dari ide.

**Primary action:** Create Project.

**Key elements:**
- Input: project name.
- Textarea: ide singkat (1–3 kalimat).
- Select: target coding agent (opsional).
- Button: Create Project.

**States:**
- Default: form kosong.
- Validation: error input.
- Processing: creating project.
- Success: redirect ke Spec Workspace.

---

## SCR-UI-03 — Spec Workspace

**User goal:** Baca dan navigasi PRD + artifacts.

**Primary action:** Navigate / Generate Build Packet.

**Key elements:**
- Left: document outline (sections).
- Center: PRD content (Markdown-like).
- Right: traceability panel (linked artifacts chips).
- Top bar: status badge, actions.

**States:**
- Default: PRD lengkap.
- Trace-gap: warning visual.
- Loading: memuat dokumen.

---

## SCR-UI-04 — Build Packet Viewer

**User goal:** Tinjau build packet dan prompt.

**Primary action:** Copy / Export / Commit.

**Key elements:**
- Milestone header (name, version, status).
- Sections: objective, scope in/out, requirements, tasks, tests.
- Agent prompt (code block with copy).
- Actions: Copy, Export, Commit.

**States:**
- Ready: packet lengkap.
- Blocked: dependencies belum siap.

---

## SCR-UI-05 — Change Impact

**User goal:** Pahami dampak revisi.

**Primary action:** Approve / Defer / Reject.

**Key elements:**
- Change request summary.
- Before/after scope.
- Affected artifacts (PRD sections, requirements, flows, screens, tasks, tests).
- Risks and version recommendation.
- Actions: Approve, Defer, Reject.

**States:**
- Default: impact normal.
- High-risk: warning menonjol.
- Approved: revisi diterapkan.

---

## SCR-UI-06 — Project Settings

**User goal:** Atur metadata dan integrasi.

**Primary action:** Save Settings.

**Key elements:**
- Project name, description.
- Target coding agent.
- Repository path.
- Visibility (private/public).

**States:**
- Default: form terisi.
- Validation: error input.
- Saved: konfirmasi tersimpan.
