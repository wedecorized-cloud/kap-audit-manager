# PRD — KAP Audit Manager (standalone)

**Product:** KAP Audit Manager  
**Lokasi:** `/Users/mymac/Documents/Accountant/kap-audit-manager`  
**Deploy:** project Vercel **terpisah** (bukan Ledgera Ops)  
**Version:** 0.1  

## Ringkasan
Workspace audit KAP: **Tahun buku → Klien → Fase KKP**, data klien, ekstrak PDF akta (PDF.js + OCR), status engagement/folder, export/import JSON.

## Bukan
- Bukan modul di dalam Ledgera Ops Vercel  
- Bukan software akuntansi / buku besar  

## MVP
- CRUD tahun & klien + search  
- Data klien lengkap + PDF extract + OCR  
- 5 folder KKP + item dokumen  
- localStorage + export/import  
- Modal/toast (bukan prompt/alert kasar)  

## Status
- Engagement: draft | in_progress | review | completed  
- Folder: empty | in_progress | complete  
- Doc item: missing | received | reviewed | final  

## Persistensi
- MVP: `localStorage` key `ledgera_audit_v1`  
- Migrate legacy `kap_companies_v8` otomatis  

## Roadmap
Phase 1 cloud DB multi-user (schema terpisah, opsional).  
