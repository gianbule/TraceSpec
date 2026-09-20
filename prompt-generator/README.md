# Prompt Generator

Folder ini adalah prompt factory TraceSpec. `templates/` menyimpan template netral; `prompts/[project]/` menyimpan prompt hasil generate yang spesifik proyek.

## Rule

- Template tidak menyimpan detail proyek.
- Prompt hasil harus memiliki YAML metadata, source paths, traceability IDs, scope in/out, acceptance criteria, stop conditions, dan response format.
- Jangan regenerate seluruh prompt saat revisi kecil; gunakan impact analysis untuk memperbarui hanya prompt yang terdampak.
