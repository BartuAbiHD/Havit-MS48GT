# Havit MS48GT

[English](README.md) | **Türkçe**

**Havit MS48GT** kablosuz mouse için Windows imleç ayarları aracı. Tek bir küçük `.exe`, kurulum yok, Python gerekmez.

**[⬇ En son sürümü indir](https://github.com/BartuAbiHD/Havit-MS48GT/releases/latest)** (`Havit-MS48GT.exe`, 64-bit Windows)

## Ne yapar?

- İmleç hızı (1-20) ve *İşaretçi duyarlılığını artır* (ivme) açık/kapalı
- Fare tekerleği kaydırma satırı ve çift tık süresi
- Sol/sağ tuşları değiştirme
- Profiller: mevcut ayarlarınızı bir isimle kaydedin, sonra tekrar yükleyin
- Pencereyi kapatınca sistem tepsisinde çalışmaya devam eder (tepsi menüsünden çıkılır)
- Diller: English, Türkçe, Azərbaycanca, Deutsch, Français, Español, Русский

> MS48GT'de DPI tuşu, yan tuş, ışık ve resmi yazılım yok, pil seviyesi de okunamıyor; yani mouse'un kendisinde ayarlanacak bir şey yok. Bu araç **Windows** imleç ayarlarını değiştirir. Ayarlar yalnızca bu mouse için değil, tüm fareler için geçerlidir.

## Kullanım

1. `Havit-MS48GT.exe` dosyasını [Releases](https://github.com/BartuAbiHD/Havit-MS48GT/releases) sayfasından indirin.
2. Çalıştırın. Bir ayarı değiştirip **Uygula**'ya basın. **Oku** Windows'taki mevcut değerleri getirir.
3. Değerleri kaydetmek için bir isim yazıp **Mevcutu kaydet**'e basın. Listeden seçip **Yükle**'ye basarak tekrar uygulayın.
4. Pencereyi kapatmak programı sistem tepsisine gizler. Açmak için tepsi simgesine sol tıklayın, kapatmak için sağ tıklayıp **Çıkış**'ı seçin.

Ayarlar `%APPDATA%\havit_ms` klasöründe (`profiles.json`, `settings.json`) tutulur. Programı sıfırlamak için bu klasörü silin.

## Windows SmartScreen uyarısı

Program kod imzalı olmadığı için Windows *"Windows bilgisayarınızı korudu"* uyarısı gösterebilir. **Daha fazla bilgi** > **Yine de çalıştır**'a tıklayın. İndirdiğiniz dosyanın orijinal olduğunu doğrulamak için SHA256 değerini sürüm notundaki ile karşılaştırın:

```powershell
Get-FileHash .\Havit-MS48GT.exe -Algorithm SHA256
```

## Gereksinimler

- Windows 10 veya 11, 64-bit
- Başka bir şey gerekmez. Python ve tüm kütüphaneler exe'nin içindedir.

## Bağlantılar

- Web sitesi: [lojitekno.tr](https://lojitekno.tr)
- Forum: [sosyal.lojitekno.tr](https://sosyal.lojitekno.tr)
- YouTube: [yton.tr/@lojitekno](https://yton.tr/@lojitekno)

## Lisans

Telif © 2026 BartuAbiHD. Tüm hakları saklıdır.

Program ücretsiz kullanılabilir. Hiçbir garanti verilmeden, "olduğu gibi" sunulur. Kaynak kodu yayınlanmamıştır; program izin alınmadan değiştirilemez, tersine çevrilemez veya yeniden dağıtılamaz. Üçüncü taraf bileşenler kendi lisanslarına tabidir, aşağıya bakın.

## Üçüncü taraf bildirimleri

`Havit-MS48GT.exe` şu açık kaynaklı bileşenleri içerir. Lisans metinleri orijinal (İngilizce) hâliyle [README](README.md#third-party-notices) dosyasındadır.

- **Dear PyGui** 2.3.1 (MIT), içinde **Dear ImGui** (MIT) bulunur: https://github.com/hoffstadt/DearPyGui
- **hidapi** (Python paketi *hidapi* 0.15.0, BSD lisansıyla kullanılır): https://github.com/trezor/cython-hidapi
- **Python** (PSF Lisansı): https://docs.python.org/3/license.html
- **PyInstaller** (GPL-2.0-or-later; onunla üretilen programların herhangi bir lisansla dağıtılmasına izin veren özel istisnayla): https://pyinstaller.org
