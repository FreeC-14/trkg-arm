# TRKG Paket Yöneticisi (ARM Sürümü)

[![Lisans: GPLv3](https://img.shields.io/badge/Lisans-GPLv3-mavi.svg)](LICENSE)

`trkg-arm.deb`, ARM tabanlı Debian sistemlerine (Termux PRoot Debian veya Raspberry Pi gibi) hafif ve kullanışlı TRKG paket yöneticisini kurmak için hazırlanmış bir `.deb` paketidir.

---

## TRKG Nedir?

**TRKG**, kullanıcı alanında özel/yerel paket yönetimi için tasarlanmış, basit ve geliştirici dostu bir paket yöneticisidir. Temel özellikleri şunlardır:

- `init`: Yeni bir paket dizini oluşturur  
- `build`: `.trkg` paket arşivleri oluşturur  
- `install`: `.trkg` paketlerini kurar  
- `remove`: Kurulu paketleri kaldırır  
- `search`: Uzak depoda paket arar  
- `upgrade`: Depodan en son paketleri indirip kurar  
- `list`: Kurulu paketleri listeler  
- `info`: Kurulu paketlerin meta verilerini gösterir  

---

## Kurulum

```bash
dpkg -i trkg-arm.deb
apt-get install -f  # Eksik bağımlılıkları düzeltmek için
