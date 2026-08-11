# PRD — Audit KKP Easy v0.2

**Prod:** https://kap-audit-manager.vercel.app  
**Path:** `/Users/mymac/Documents/Accountant/kap-audit-manager`  
**Deploy:** Vercel project **kap-audit-manager** (bukan Ledgera Ops)

## Positioning (dari SWOT)
Engagement cockpit untuk KAP Indonesia — **bukan** MindBridge (full-population AI) atau DataSnipper (Excel evidence).  
Teman kerja harian: langkah, risiko ringkas, PBC, bukti ber-sumber, draf.

Lihat: `docs/SWOT-AI-AUDIT-TOOLS.md`

## UX
- **2 layar saja:** Daftar klien ↔ Detail klien  
- Tahun = filter chip, bukan folder navigasi  
- Auto-save localStorage (`kap_audit_easy_v2`)  
- Strip **Fokus hari ini**  

## Modul detail (tabs)
1. **Langkah** — 5 step centang (info → pra → risiko → kerja → lapor)  
2. **Risiko** — 5 pertanyaan → skor 0–10 (risk signal lite)  
3. **Minta dokumen (PBC)** — open / diterima  
4. **Bukti** — judul + sumber + langkah (evidence linkage lite)  
5. **Asisten draf** — template ringkasan (bukan opini)  

## Non-goals
Full GL ML · Excel add-in · multi-user cloud (nanti) · ganti software akuntansi  

## Disclaimer
Skor & draf **wajib direview manusia**.  
