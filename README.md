# IDT Knowledge Graph

Obsidian/Quartz knowledge vault cho môn **IDT (BUSM7045) — MBA WSU**, dựa trên giáo trình:

> **Digital Business and E-Commerce Management** — Dave Chaffey, Tanya Hemphill & David Edmundson-Bird, 8th Edition (Pearson).

## Cấu trúc

- `content/00_MOC/` — Map of Content tổng quan toàn sách
- `content/01..10_*/` — 10 chapter notes theo 3 Part (Introduction / Strategy and applications / Implementation)
- `content/Key_Concepts/` — Các khái niệm chính (định nghĩa theo Glossary của sách)
- `content/Cases/` — Case study và mini case study với số liệu từ sách

## Sử dụng

Mở folder này (hoặc `content/`) làm Obsidian vault. Ghi chú viết tiếng Việt, giữ nguyên thuật ngữ tiếng Anh, liên kết bằng wikilink.

Build web (Quartz):

```bash
npm ci
npx quartz build --serve
```
