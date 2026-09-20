# Test Plan — TraceSpec

| ID | Requirement | Scenario | Expected result |
|---|---|---|---|
| TEST-01 | FR-01 | Ide minim konteks | Sistem merangkum dan meminta klarifikasi prioritas |
| TEST-02 | FR-02 | Ide dengan scope terlalu besar | Sistem mengusulkan MVP dan non-goals |
| TEST-03 | FR-03 | PRD dibuat | Semua requirement memiliki ID dan links yang diperlukan |
| TEST-04 | FR-04 | Generate build packet | Packet memuat scope, task, tests, dan stop conditions |
| TEST-05 | FR-05 | User mengubah requirement | Sistem menampilkan artefak terdampak sebelum edit |
| TEST-06 | NFR-03 | User belum approve push | Tidak ada file GitHub yang ditulis |
| TEST-07 | NFR-04 | Traceability audit | Hubungan hilang diberi label [TRACE GAP] |
