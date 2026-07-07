# VERİTABANI
- Temel anlamda verileri listeler halinde tablo ve satırlarda tutan her yapı aslında kendi çapında veritabanıdır.
---
## Veritabanı Yönetim Sistemi
- Network üzerinde belli bir portu dinleyip kendisine gelen SQL komutlarını kendi kaynaklarını kullanarak çalıştıran ve aynı anda birden fazla istemciye hizmet veren veritabanı sistemlerine veritabanı yönetim sistemi denir.
---
## Veritabanı Sunucu
- Microsoft SQL Server, Oracle, PostgreSQL birer veritabanı sunucu yazılımıdır. Networkten gelen koumtları dinleyen ve bu komutlardan gelen isteklere göre kendi kaynaklarını kullanarak sonucu döndüren bir mekanizma.
---

# SQL
- (**S**tructured **Q**uery **L**anguage) (Yapısal Sorgulama Dili)





```mermaid
flowchart TB
    VB[Veri Bilimi]
    V[Veri]
    VO[Veri Önişleme]
    VV[Veritabanlarından Veri Çekme]
    KVT[Kirli Veriyi Temizleme]
    B[Bilim]
    K[Kütüphaneler]
    A[Algoritmalar]
    PR[Python, R]

    %% Yukarıdan aşağı
    VB --> V
    VB --> B

    V --> VO
    VO --> VV
    VO --> KVT

    B --> K
    B --> A
    B --> PR

```
