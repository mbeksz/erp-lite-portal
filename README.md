# ERP Lite Tablet Portalı

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/MSSQL-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Durum-Canlıda-brightgreen?style=flat-square" />
  <img src="https://img.shields.io/badge/Tür-Özel%20Kurumsal%20Yazılım-blue?style=flat-square" />
</p>

---

> Bu proje bir otomotiv bayilik grubu için özel kurumsal yazılım olarak geliştirilmiştir.
> Bu repo yalnızca proje yapısını ve dokümantasyonu **portfolyo amaçlı** paylaşmaktadır. Kaynak kod dahil edilmemiştir.

---

## Genel Bakış

Mevcut ERP sistemi atölye personelinin tablet üzerinden hızlı kullanımına uygun değildir — sipariş bilgilerine ulaşmak için gereksiz pek çok ekranı geçmek gerekmekteydi. Bu sorunu çözmek amacıyla **ERP veritabanına doğrudan bağlanan**, atölye kullanımı için sadeleştirilmiş bir ara portal geliştirilmiştir.

Kullanıcılar iş emri numarasını girerek kumaş, nakış, aksesuar, numune kriterleri ve renk-beden bilgilerine **tek ekrandan** ulaşabilir; fotoğraf ve belgeleri doğrudan iş emri kaydına yükleyebilir.

---

<img width="1312" height="729" alt="Adsız tasarım (3)" src="https://github.com/user-attachments/assets/eb53fc88-5586-40db-8439-40cb5e143a88" />


## Teknoloji Yığını

```
Backend    → Node.js · Express.js
Frontend   → React · TypeScript · Vite
Veritabanı → MSSQL (ERP doğrudan bağlantı)
```

---

## Mimari

```
backend/
├── src/
│   ├── index.js
│   ├── routes/          # API route'ları
│   ├── controllers/     # İş emri, sipariş, dosya yükleme mantığı
│   ├── services/        # ERP veritabanı sorguları
│   ├── config/          # Veritabanı bağlantı ayarları
│   └── temp_uploads/    # Geçici dosya yükleme dizini

frontend/
├── src/
│   ├── App.tsx
│   ├── components/
│   └── services/
```

---

## Temel Özellikler

- İş emri numarasıyla tek ekrandan tüm sipariş detaylarına erişim
- Tablet optimizasyonlu sade arayüz
- Fotoğraf, teknik çizim ve belge yükleme — ERP kaydına anlık eşleştirme
- Mevcut ERP sistemini değiştirmeden üzerine katman olarak çalışır
- Doğrudan ERP veritabanı bağlantısı — gerçek zamanlı veri


