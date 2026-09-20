# TraceSpec Prompt Contract

Setiap prompt wajib memiliki: (1) `prompt_id`, type, version, target tool/agent, status, dan source; (2) objective yang terukur; (3) dokumen yang harus dibaca; (4) traceability IDs; (5) scope in/out; (6) acceptance criteria; (7) constraints; (8) stop conditions; dan (9) format respons.

Prompt implementasi wajib meminta agent membaca sumber, membuat plan sebelum coding, membatasi perubahan pada task aktif, menjalankan/menulis test, dan melaporkan file berubah serta limitation.
