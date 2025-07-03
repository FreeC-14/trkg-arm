<p align="center">
<pre>
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠤⣴⣶⣶⣶⣶⣦⣤⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⣀⣴⣾⣿⣶⣄⠈⠻⣿⣿⣿⣿⣿⣿⡀⢰⣦⣀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⢠⣾⣿⣿⣿⣿⣿⣿⣿⣷⣤⡀⠙⢿⣿⣿⣿⡇⠀⣿⣿⣷⡄⠀⠀⠀
⠀⠀⠀⡰⠿⠿⠿⠿⠛⠛⠛⠛⠋⠉⠉⠀⠀⠈⠻⣿⡇⠀⣿⣿⣿⣿⣆⠀⠀⠀
⠀⠀⣀⣤⣤⣤⣤⣴⣶⠖⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠁⠀⣿⣿⣿⣿⡿⠂⠀⠀
⠀⢀⣿⣿⣿⣿⣿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢹⣿⣿⠋⢀⣴⡀⠀
⠀⢸⣿⣿⣿⡿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⠟⠁⣠⣾⣿⡇⠀
⠀⢸⣿⣿⠋⢀⣴⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣾⣿⣿⣿⡇⠀
⠀⠈⠟⠁⣠⣿⣿⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣿⣿⣿⣿⣿⠁⠀
⠀⠀⠠⣾⣿⣿⣿⣿⠀⢠⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠴⠿⠿⠟⠛⠛⠛⠋⠀⠀
⠀⠀⠀⠹⣿⣿⣿⣿⠀⢸⣿⣦⣄⠀⠀⣀⣀⣀⣤⣤⣤⣤⣤⣶⣶⣶⠆⠀⠀⠀
⠀⠀⠀⠀⠘⢿⣿⣿⡄⠸⣿⣿⣿⣷⣄⡈⠙⢿⣿⣿⣿⣿⣿⣿⡿⠃⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠉⠻⠇⠀⣿⣿⣿⣿⣿⣿⣦⡀⠉⠻⣿⡿⠟⠉⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠛⠻⠿⠿⠿⠟⠓⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
</pre>
</p>

## TRKG Özellikleri

```bash
# Temel Kullanım
trkg [komut] [seçenekler] [argümanlar]
```

### Komut Referansı
| Komut       | Kullanım                      | Açıklama                     |
|-------------|-------------------------------|------------------------------|
| `init`      | `trkg init <paket-adı>`       | Yeni paket şablonu oluşturur |
| `build`     | `trkg build <yol>`            | Paket derleme                |
| `install`   | `trkg install <paket.deb>`    | Paket kurulumu               |
| `remove`    | `trkg remove <paket-adı>`     | Paket kaldırma               |
| `search`    | `trkg search <anahtar-kelime>`| Paket arama                  |
| `upgrade`   | `trkg upgrade`                | Tüm paketleri güncelle       |
| `list`      | `trkg list [--installed]`     | Paket listeleme              |
| `info`      | `trkg info <paket-adı>`       | Paket detayları              |

---

##  Sistem Gereksinimleri

### Zorunlu Bağımlılıklar
```bash
# Debian/Ubuntu
sudo apt update && sudo apt install -y \
    libcurl4-openssl-dev \
    libssl-dev \
    libcjson-dev \
    openssl
```

### Minimum Versiyonlar
| Paket       | Versiyon  | Kontrol Komutu               |
|-------------|-----------|------------------------------|
| OpenSSL     | ≥ 1.1.x   | `openssl version`            |
| libcurl     | ≥ 7.64.0  | `curl --version`             |
| libcjson    | ≥ 1.7.14  | `dpkg -l libcjson-dev`       |

---

##  Lisans Bilgisi

```text
TRKG - Hafif ARM Paket Yöneticisi
Copyright (C) 2023 dreamtech.dev & FreeC-14

Bu program özgür yazılımdır: GNU GPL v3 lisansı ile dağıtılmaktadır.
Bu programın yararlı olacağı umulur ancak HİÇBİR GARANTİ VERMEZ.
```

**Tam lisans metni:** [LICENSE dosyasını inceleyin](LICENSE)

---

##  Katkı Süreci

1. **Depoyu Forklayın**  
   [GitHub Fork butonuna tıklayarak](https://github.com/dreamtech-dev/trkg-arm/fork)

2. **Geliştirme Yapın**  
   ```bash
   git clone https://github.com/sizin-kullanici-adi/trkg-arm.git
   cd trkg-arm
   git checkout -b yeni-ozellik
   ```

3. **Değişiklikleri Gönderin**  
   ```bash
   git add .
   git commit -m "Yeni özellik: xyz eklendi"
   git push origin yeni-ozellik
   ```

4. **Pull Request Açın**  
   GitHub üzerinden ana depoya PR gönderin

---

##  Sorun Giderme

### Sık Karşılaşılan Sorunlar

**Hata:** `Bağımlılıklar karşılanamadı`
```bash
# Çözüm:
sudo apt --fix-broken install
```

**Hata:** `ARM mimari uyumsuzluğu`
```bash
# Kontrol edin:
dpkg --print-architecture
uname -m
```

**Hata:** `İzin reddedildi`
```bash
# Çözüm:
sudo chmod +x /usr/local/bin/trkg
```

---

##  İletişim & Destek

| Platform       | Bağlantı                              |
|----------------|---------------------------------------|
| GitHub Issues  | [Yeni Issue Aç](https://github.com/freec-14/trkg-arm/issues) |
| E-posta        | sussyarch@proton.me               |
| Discord        | [Sunucuya Katıl](https://discord.gg/mEYASMKRkn) |

[![TRKG Build Status](https://img.shields.io/github/actions/workflow/status/dreamtech-dev/trkg-arm/build.yml?label=Build&style=for-the-badge)](https://github.com/dreamtech-dev/trkg-arm/actions)

---

> **dreamtech.dev** & **FreeC-14** ekibi tarafından geliştirilmiştir  
> Son güncelleme: ![](https://img.shields.io/github/last-commit/dreamtech-dev/trkg-arm?color=blue&label=Güncelleme&style=flat-square)
```
