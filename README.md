# Faceix — Resmî Dağıtım ve İndirme Merkezi

**Faceix**, okul öğretmenleri, idareciler ve kurumlar için tasarlanmış; **%100 çevrimdışı (offline)** çalışan **Yüz Koru (KVKK Yüz Kapatma)** ve **E-Okul Vesikalık** masaüstü uygulamasının derlenmiş kurulum paketlerini barındırır.

> **Önemli Not:** Bu depo yalnızca son kullanıcı kurulum paketlerinin (**Releases**) dağıtımı içindir. Uygulamanın kaynak kodu kapalı/özel mülkiyettir (**All Rights Reserved — `ixlab.tr`**).

---

## 📥 İndirme

En güncel sürüm paketlerini sağ taraftaki **[Releases](../../releases)** bölümünden indirebilirsiniz:

| İşletim Sistemi | Paket Dosyası | Kurulum / Çalıştırma Notu |
|---|---|---|
| **Windows 10/11 (64-bit)** | `Faceix_Setup_v*.exe` | Kurulum sihirbazı (İmzasız sürümde SmartScreen *"Ek bilgi → Yine de çalıştır"* gerekebilir) |
| **Windows (Taşınabilir)** | `Faceix_v*_Windows_Portable.zip` | ZIP'i çıkarıp `Faceix.exe` çalıştırın (yönetici izni gerekmez) |
| **Pardus 23 / Debian 12+ (amd64)** | `faceix_*_amd64.deb` | `sudo apt install ./faceix_*_amd64.deb` |
| **Linux (Taşınabilir)** | `Faceix_v*_Linux_Pardus_Portable.tar.gz` | Arşivi açıp içindeki `Faceix` çalıştırılabilir dosyasını başlatın |
| **macOS (Apple Silicon)** | `Faceix_v*_macOS_arm64.dmg` / `.zip` | `Faceix.app` dosyasını `Applications` klasörüne sürükleyin (İmzasız sürümde ilk açılışta *Sağ tık → Aç* kullanın) |

---

## 🔒 Bütünlük Doğrulaması (`SHA256SUMS.txt`)

Her sürümde yer alan `SHA256SUMS.txt` dosyası ile indirdiğiniz paketin bütünlüğünü doğrulayabilirsiniz:

- **Windows (PowerShell):**
  ```powershell
  Get-FileHash .\Faceix_Setup_v*.exe -Algorithm SHA256
  ```
- **Linux / Pardus / macOS:**
  ```bash
  sha256sum -c SHA256SUMS.txt --ignore-missing
  ```

---

## ⚖️ Lisans ve Gizlilik

- **Faceix Uygulama Paketi:** Tüm hakları saklıdır (`ixlab.tr`). Telif hakkı sahibinin izni olmaksızın kaynak kod elde etme amaçlı tersine mühendislik ve ticari yeniden dağıtım yasaktır.
- **Üçüncü Taraf Açık Kaynak Bileşenler ve Modeller:** Dahil edilen açık kaynak kütüphaneler (`PySide6` LGPL-3.0, `OpenCV` Apache-2.0, `YuNet` MIT, `SFace` Apache-2.0 vb.) kendi lisans koşullarına tabidir; ayrıntılar için [LICENSES.md](LICENSES.md) dosyasına bakın.
- **İletişim:** `ixlabtr@gmail.com` · [https://ixlab.tr](https://ixlab.tr)
