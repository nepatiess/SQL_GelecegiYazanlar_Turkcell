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

---
## Neden SQL?
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
---
# İlişkisel Veritabanı Kavramı (RDMS)
- Tekrar eden verileri tekilleştirmek amacıyla kullanılan veritabanı sistemleridir.

<p align="center">
  <img src="https://raw.githubusercontent.com/nepatiess/SQL_GelecegiYazanlar_Turkcell/refs/heads/main/images/RDMS.png" width="600">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nepatiess/SQL_GelecegiYazanlar_Turkcell/refs/heads/main/images/%C4%B0li%C5%9FkiselVT%C3%96rnek.png" width="600">
</p>

---
# Sanal Makine Kavramı
- Fiziksel bir işletim sisteminin içinde başka işletim sistemlerinin de gerçek birer bilgisayar gibi çalıştırılması kavramıdır.

- Öncesinde:
```mermaid
flowchart TB
    FIS[Fiziksel Server]
    WS[Web Server]
    DS[Database Server]
    FS[File Server]
    MS[Mail Server]
    AS[Application Server]

    %% Yukarıdan aşağı
    FIS --> WS
    FIS --> DS
    FIS --> FS
    FIS --> MS
    FIS --> AS

```

- Sonrasında:
```mermaid
flowchart TB
    FIS1[Fiziksel Server 1]
    FIS2[Fiziksel Server 2]
    FIS3[Fiziksel Server 3]
    FIS4[Fiziksel Server 4]
    FIS5[Fiziksel Server 5]

    WS[Web Server]
    DS[Database Server]
    FS[File Server]
    MS[Mail Server]
    AS[Application Server]

    %% Yukarıdan aşağı
    FIS1 --> WS
    FIS2 --> DS
    FIS3 --> FS
    FIS4 --> MS
    FIS5 --> AS

```

```mermaid
flowchart TB
    FIZ[Fiziksel Server]
    SS1[Sanal Server 1]
    SS2[Sanal Server 2]
    SS3[Sanal Server 3]
    SS4[Sanal Server 4]
    SS5[Sanal Server 5]

    WS[Web Server]
    DS[Database Server]
    FS[File Server]
    MS[Mail Server]
    AS[Application Server]

    %% Yukarıdan aşağı
    FIZ --> SS1
    SS1 --> WS

    FIZ --> SS2
    SS2 --> DS

    FIZ --> SS3
    SS3 --> FS

    FIZ --> SS4
    SS4 --> MS

    FIZ --> SS5
    SS5 --> AS

```

















