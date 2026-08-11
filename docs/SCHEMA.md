# Schema — KAP Audit Manager

## localStorage `ledgera_audit_v1`

```ts
type Store = { version: 1; companiesByYear: Record<string, Company[]> };

type Company = {
  id: string;
  name: string;
  address: string;
  city: string;
  director: string;
  position: string;
  commissioner: string;
  npwp: string;
  nib: string;
  legalForm: string;
  aktaNo: string;
  aktaDate: string;
  modalDasar: string;
  modalDisetor: string;
  engagementPartner: string;
  engagementManager: string;
  status: "draft" | "in_progress" | "review" | "completed";
  notes: string;
  folders: Record<FolderKey, { status: FolderStatus; items: DocItem[] }>;
  createdAt: string;
  updatedAt: string;
};

type FolderKey =
  | "Pre Engagement"
  | "Risk Assessment"
  | "Risk Response"
  | "Completing & Reporting"
  | "Arsip KKP";

type DocItem = {
  id: string;
  title: string;
  note: string;
  status: "missing" | "received" | "reviewed" | "final";
  updatedAt: string;
};
```

## Extract field map
Nama Perusahaan→name · Kedudukan→city · Direktur→director · Komisaris→commissioner · Nomor/Tanggal Akta · Modal dasar/disetor  
