---
project: TraceSpec
version: v0.1
status: Draft
source_prd: docs/product/tracespec/PRD.md
---

# Project Context

TraceSpec adalah AI Product-to-Build Orchestrator. Produk membuat hubungan problem → goal → requirement → flow → screen → task → test agar planning AI coding dapat ditinjau, direvisi, dan dieksekusi secara terkontrol.

## MVP boundaries

In scope: discovery, challenge mode, traceable PRD, flow/screen blueprint, task slicing, build packet, trace audit, change impact.

Out of scope: visual editor penuh, eksekusi kode langsung, enterprise PM, marketplace, dan integrasi real-time banyak agent.

## Non-negotiable rules

- Jangan menambah feature di luar scope.
- Jangan mengarang fakta atau requirement.
- Jangan mengubah artefak tidak terkait task aktif.
- Requirement penting harus memiliki acceptance criteria dan test.
- Berhenti saat menemukan ambiguity atau [TRACE GAP] kritis.
