# 🎨 PhotoGIMP

<img src="../.local/share/icons/hicolor/256x256/256x256.png" align="right" alt="PhotoGIMP uygulama simgesi" title="PhotoGIMP uygulama simgesi">

[![GitHub yıldızları](https://img.shields.io/github/stars/Diolinux/PhotoGIMP?style=social)](https://github.com/Diolinux/PhotoGIMP)
[![Lisans: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![En Son Sürüm](https://img.shields.io/github/v/release/Diolinux/PhotoGIMP)](https://github.com/Diolinux/PhotoGIMP/releases/latest)

**PhotoGIMP**, [GIMP'i](https://www.gimp.org/) (GNU Image Manipulation Program) **Adobe Photoshop** kullanıcılarına tanıdık gelecek bir düzene dönüştüren, ücretsiz ve topluluk tarafından geliştirilen bir yamadır. Photoshop'tan GIMP'e geçiyor ve kendinizi ilk andan itibaren alışık olduğunuz bir ortamda hissetmek istiyorsanız PhotoGIMP tam size göre.

> **GIMP'i ilk kez mi kullanıyorsunuz?** GIMP; Linux, macOS ve Windows için sunulan ücretsiz ve açık kaynaklı bir görüntü düzenleyicidir. Fotoğraf düzeltme, görüntü birleştirme, grafik tasarım ve daha fazlası dahil olmak üzere Photoshop'un yapabildiği çoğu şeyi tamamen ücretsiz olarak yapabilir. PhotoGIMP yalnızca GIMP'in _görünümünü ve kullanımını_ Photoshop'a daha çok benzetir.

---

## ✨ Özellikler

- **Photoshop benzeri araç düzeni** — Araçlar, Adobe Photoshop'ta alışık olduğunuz konumları taklit edecek şekilde yeniden düzenlenmiştir.
- **Özel açılış ekranı** — Başlangıçta sizi PhotoGIMP'e özel bir açılış ekranı karşılar.
- **En geniş tuval alanı** — Varsayılan ayarlar, mümkün olan en geniş çalışma alanını sağlamak üzere optimize edilmiştir.
- **Photoshop klavye kısayolları** — Klavye kısayolları, Windows sürümü için [Adobe'nin resmî belgelerini](https://helpx.adobe.com/photoshop/using/default-keyboard-shortcuts.html) temel alır.
- **Özel simge ve ad** — PhotoGIMP, özel bir `.desktop` dosyası sayesinde sistem menünüzde kendi simgesi ve uygulama adıyla görünür.

---

## 📷 Ekran Görüntüleri

| Açılış Ekranı | Uygulama Penceresi |
|-|-|
| ![[PhotoGIMP Diolinux açılış ekranı]](../.config/GIMP/3.0/splashes/splash-screen-2025-v2.png)<br>PhotoGIMP Diolinux açılış ekranı | ![[PhotoGIMP 3]](../screenshots/photogimp_3_-_diolinux.png)<br>PhotoGIMP 3

---

## 📋 Gereksinimler

PhotoGIMP'i kurmadan önce aşağıdakileri yerine getirdiğinizden emin olun:

| Gereksinim                         | Ayrıntılar                                                                                                                                                                       |
| ---------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **GIMP 3.0 veya daha yeni bir sürüm** | [gimp.org](https://www.gimp.org/downloads/) veya [Flathub](https://flathub.org/apps/org.gimp.GIMP) (Linux) üzerinden indirin                                                    |
| **GIMP'i en az bir kez çalıştırın** | PhotoGIMP'in üzerine yazabilmesi için GIMP'in önce yapılandırma dosyalarını oluşturması gerekir. **GIMP'i kurun → açın → kapatın → ardından PhotoGIMP'i kurun.**                  |

---

## ⚙ Kurulum

> [!WARNING]
> **Kurulumdan önce mevcut GIMP ayarlarınızı yedekleyin!** PhotoGIMP, GIMP'in yapılandırma dosyalarının üzerine yazar. Korumak istediğiniz özel ayarlarınız varsa önce bir yedek kopya oluşturun. Aşağıdaki her bölümde yer alan yedekleme talimatlarına bakın.

---

### 🐧 Flatpak (Linux)

<img src="https://skillicons.dev/icons?i=linux" align="right" width="40" />

#### Yedekleme (isteğe bağlı)

Mevcut GIMP ayarlarınızı korumak istiyorsanız önce yedekleyin:

```bash
cp -r ~/.config/GIMP/3.0 ~/GIMP-3.0-backup
```

#### Kurulum

1. GIMP'i daha önce [Flathub üzerinden](https://flathub.org/apps/org.gimp.GIMP) kurduğunuzdan emin olun.
2. **GIMP'i bir kez açıp kapatın** — bu işlem PhotoGIMP'in ihtiyaç duyduğu yapılandırma klasörlerini oluşturur.
3. En son sürümü indirin:
   👉 **[Linux için PhotoGIMP'i indirin (.zip)](https://github.com/Diolinux/PhotoGIMP/releases/download/3.0/PhotoGIMP-linux.zip)**
4. `.zip` dosyasını **ana klasörünüze** (`~`) çıkarın.
    - Bu işlem dosyaları gizli klasörler olan `~/.config` ve `~/.local` içine yerleştirir.
    - Dosya yöneticinizde gizli klasörleri görmek için <kbd>Ctrl</kbd> + <kbd>H</kbd> tuşlarına basın.
    - Mevcut dosyalarla ilgili bir soru görüntülendiğinde **"Değiştir"** veya **"Üzerine yaz"** seçeneğini belirleyin.
5. GIMP'i açın — yeni PhotoGIMP düzenini görmelisiniz! 🎉

<details>
<summary><strong>💡 Flatpak dışındaki bir GIMP sürümünü mü kullanıyorsunuz?</strong></summary>

GIMP'i Flatpak yerine dağıtımınızın paket yöneticisinden (apt, dnf, pacman vb.) kurduysanız yapılandırma klasörü yine aynı konumdadır (`~/.config/GIMP/3.0`); dolayısıyla yukarıdaki adımlar geçerlidir. Yalnızca GIMP 3.0 veya daha yeni bir sürümü kullandığınızdan emin olun.

</details>

---

### 🪟 Windows

<img src="https://skillicons.dev/icons?i=windows" align="right" />

#### Yedekleme (isteğe bağlı)

Mevcut GIMP ayarlarınızı korumak istiyorsanız önce yedekleyin:

1. Çalıştır iletişim kutusunu açmak için <kbd>Windows</kbd> + <kbd>R</kbd> tuşlarına basın.
2. `%APPDATA%\GIMP` yazıp <kbd>Enter</kbd> tuşuna basın.
3. `3.0` klasörünün tamamını güvenli bir konuma (örneğin Masaüstünüze) kopyalayın.

#### Kurulum

1. [GIMP'i resmi web sitesinden](https://www.gimp.org/downloads/) kurduğunuzdan emin olun.
2. **GIMP'i bir kez açıp kapatın** — bu işlem PhotoGIMP'in ihtiyaç duyduğu yapılandırma klasörlerini oluşturur.
3. En son sürümü indirin:
   👉 **[Windows için PhotoGIMP'i indirin (.zip)](https://github.com/Diolinux/PhotoGIMP/releases/download/3.0/PhotoGIMP.zip)**
4. `PhotoGIMP.zip` dosyasının içeriğini istediğiniz bir klasöre (örneğin Masaüstünüze) çıkarın.
5. Çıkardığınız klasörü açın ve **`3.0` klasörünü kopyalayın**.
6. Çalıştır iletişim kutusunu açmak için <kbd>Windows</kbd> + <kbd>R</kbd> tuşlarına basın.
7. `%APPDATA%\GIMP` yazıp <kbd>Enter</kbd> tuşuna basın — GIMP'in ayarlar klasörü açılır.
8. `3.0` klasörünü buraya **yapıştırın**.
9. Mevcut dosyalarla ilgili bir soru görüntülendiğinde **"Hedefteki dosyaları değiştir"** seçeneğini belirleyin.
10. GIMP'i açın — yeni PhotoGIMP düzenini görmelisiniz! 🎉

<details>
<summary><strong>💡 İsteğe bağlı: GIMP kısayolunun simgesini değiştirin</strong></summary>

Ayrıca [photogimp.ico](https://github.com/Diolinux/PhotoGIMP/releases/download/3.0/photogimp.ico) dosyasını indirip şu konumdaki GIMP kısayolunun simgesini değiştirebilirsiniz:

```
%appdata%\Microsoft\Windows\Start Menu\Programs\GIMP 3.0.0
```

Kısayola sağ tıklayın → **Özellikler** → **Simge Değiştir** → indirdiğiniz `.ico` dosyasını seçin.

</details>

<details>
<summary><strong>🍫 Chocolatey ile kurulum (alternatif)</strong></summary>

[Chocolatey](https://chocolatey.org/) kullanıyorsanız PhotoGIMP'i tek bir komutla kurabilirsiniz:

```powershell
choco install photogimp
```

Bakımını yapan: [André Augusto](https://github.com/AndreAugustoDev)

</details>

---

### 🍎 macOS

<img src="https://skillicons.dev/icons?i=macos" align="right" />

#### Yedekleme (isteğe bağlı)

Mevcut GIMP ayarlarınızı korumak istiyorsanız önce yedekleyin:

1. Finder'ı açın.
2. <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>G</kbd> tuşlarına basıp `~/Library/Application Support/GIMP` konumuna gidin.
3. `GIMP` klasörünün tamamını güvenli bir konuma (örneğin Masaüstünüze) kopyalayın.

#### Kurulum

1. [GIMP'i resmi web sitesinden](https://www.gimp.org/downloads/) kurduğunuzdan emin olun.
2. **GIMP'i bir kez açıp kapatın** — bu işlem PhotoGIMP'in ihtiyaç duyduğu yapılandırma klasörlerini oluşturur.
3. En son sürümü indirin:
   👉 **[macOS için PhotoGIMP'i indirin (.zip)](https://github.com/Diolinux/PhotoGIMP/releases/download/3.0/PhotoGIMP.zip)**
4. `PhotoGIMP.zip` dosyasının içeriğini istediğiniz bir klasöre (örneğin Masaüstünüze) çıkarın.
5. Çıkardığınız klasörü açın ve **`3.0` klasörünü kopyalayın**.
6. Finder'ı açın, "Klasöre Git" penceresini açmak için <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>G</kbd> tuşlarına basın.
7. `~/Library/Application Support/GIMP` yazıp <kbd>Enter</kbd> tuşuna basın.
8. Önceki bir kurulumdan kalma `2.10` klasörü görürseniz çakışmaları önlemek için **silin**.
9. `3.0` klasörünü GIMP klasörünün içine **yapıştırın**.
10. Mevcut dosyalarla ilgili bir soru görüntülendiğinde **"Değiştir"** veya **"Birleştir"** seçeneğini belirleyin.
11. GIMP'i açın — yeni PhotoGIMP düzenini görmelisiniz! 🎉

<details>
<summary><strong>Alternatif: Terminal ile kurulum</strong></summary>

Finder'daki **"Birleştir"** seçeneği mevcut dosyaları sessizce atlıyorsa veya komut satırını tercih ediyorsanız PhotoGIMP dosyalarını `rsync` ile kopyalayabilirsiniz.

1. Terminal'i açın.
2. `/path/to/extracted/3.0/` bölümünü çıkardığınız `3.0` klasörünün konumuyla değiştirerek `rsync` komutunu çalıştırın:

   ```bash
   rsync -av --ignore-times /path/to/extracted/3.0/ ~/Library/Application\ Support/GIMP/3.0/
   ```

   Her iki yolun da `/` ile bittiğinden emin olun.
3. Kurulu GIMP sürümünüz farklı bir sürüm klasörü kullanıyorsa hedef yolu buna göre değiştirin (örneğin GIMP 3.2 için `~/Library/Application\ Support/GIMP/3.2/` kullanın).

</details>

---

## 📦 Yamanın İçeriği

PhotoGIMP, GIMP'in yapılandırma dizinindeki şu dosyaları değiştirir veya bu dizine ekler:

| Dosya / Klasör | İşlevi                                             |
| --------------- | -------------------------------------------------- |
| `shortcutsrc`   | Klavye kısayollarını Photoshop ile eşleşecek şekilde ayarlar |
| `toolrc`        | Araç yapılandırmasını ve sıralamasını belirler     |
| `sessionrc`     | Pencere düzenini ve panel konumlarını belirler     |
| `dockrc`        | Sabitlenebilir iletişim kutusu/panel yapılandırmasını belirler |
| `gimprc`        | Genel GIMP tercihlerini (tuval, ızgara vb.) belirler |
| `contextrc`     | Etkin araç/renk bağlamı ayarlarını belirler        |
| `splashes/`     | Özel PhotoGIMP açılış ekranını içerir              |
| `theme.css`     | Küçük kullanıcı arayüzü tema düzenlemelerini içerir |
| `templaterc`    | Önceden tanımlanmış tuval şablonlarını içerir      |

Yama, Linux'ta ayrıca şunları kurar:

- Özel bir `.desktop` dosyası (PhotoGIMP adı ve simgesine sahip uygulama başlatıcısı)
- `~/.local/share/icons/` içine özel bir uygulama simgesi

---

## 🗑 Kaldırma

PhotoGIMP'i kaldırıp GIMP'i varsayılan durumuna döndürmek için GIMP'in yapılandırma klasörünü silmeniz ve GIMP'i yeniden açmanız yeterlidir. GIMP, yeni varsayılan ayarları otomatik olarak oluşturur.

### Linux

```bash
rm -rf ~/.config/GIMP/3.0
```

Ardından GIMP'i yeniden açın — yepyeni bir varsayılan yapılandırma oluşturulur.

Daha önce yedek aldıysanız bunun yerine yedeğinizi geri yükleyin:

```bash
cp -r ~/GIMP-3.0-backup ~/.config/GIMP/3.0
```

### Windows

1. <kbd>Windows</kbd> + <kbd>R</kbd> tuşlarına basın, `%APPDATA%\GIMP` yazın ve <kbd>Enter</kbd> tuşuna basın.
2. `3.0` klasörünü silin.
3. GIMP'i açın — varsayılan ayarlar yeniden oluşturulur.

Alternatif olarak yedeklediğiniz `3.0` klasörünü yeniden yapıştırarak yedeğinizi geri yükleyin.

### macOS

1. Finder'ı açın ve <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>G</kbd> tuşlarına basın.
2. `~/Library/Application Support/GIMP` konumuna gidin.
3. `3.0` klasörünü silin.
4. GIMP'i açın — varsayılan ayarlar yeniden oluşturulur.

Alternatif olarak yedeklediğiniz klasörü yeniden yapıştırarak yedeğinizi geri yükleyin.

---

## ❓ Sorun Giderme / SSS

> [!CAUTION]
> **PhotoGIMP'in resmi bir web sitesi yoktur.** Projenin tek resmi kaynağı GitHub reposudur: https://github.com/Diolinux/PhotoGIMP/

<details>
<summary><strong>PhotoGIMP hiçbir şeyi değiştirmedi — GIMP aynı görünüyor</strong></summary>

- Dosyaları **doğru konuma** çıkardığınızdan emin olun. En sık yapılan hata, dosyaları yanlış klasöre çıkarmaktır.
- **Linux**: `.config` ve `.local` klasörleri ana dizininizde (`~`) bulunmalıdır. Bu klasörler gizlidir; dosya yöneticinizde görmek için <kbd>Ctrl</kbd> + <kbd>H</kbd> tuşlarına basın.
- **Windows**: `3.0` klasörü `%APPDATA%\GIMP` klasörünün yanında değil, içinde olmalıdır.
- **macOS**: `3.0` klasörü `~/Library/Application Support/GIMP` klasörünün içinde olmalıdır.
- Dosyaları yapıştırmadan önce **GIMP'i kapattınız mı?** GIMP, kapanırken yeni eklenen ayarların üzerine yazabilir.
  </details>

<details>
<summary><strong>PhotoGIMP'i kurduktan sonra GIMP'i açarken hata alıyorum</strong></summary>

- Bu durum genellikle GIMP sürümünün eşleşmediği anlamına gelir. PhotoGIMP, **GIMP 3.0+** için hazırlanmıştır. GIMP 2.x kullanıyorsanız uyumlu olmayacaktır.
- Yapılandırma klasörünü silip yeniden kurmayı deneyin — [Kaldırma](#-kaldırma) bölümüne bakın.
  </details>

<details>
<summary><strong>PhotoGIMP'i GIMP 2.10 ile kullanabilir miyim?</strong></summary>

Hayır. PhotoGIMP'in bu sürümü yalnızca **GIMP 3.0 ve daha yeni sürümler** için tasarlanmıştır. Yapılandırma biçimi GIMP 2.x ile 3.x arasında önemli ölçüde değişmiştir.

</details>

<details>
<summary><strong>PhotoGIMP özel fırçalarımı, yazı tiplerimi veya eklentilerimi siler mi?</strong></summary>

Hayır. PhotoGIMP yalnızca yapılandırma dosyalarını (kısayollar, düzen, tercihler) değiştirir. Kişisel fırçalarınıza, yazı tiplerinize, renk geçişlerinize ve eklentilerinize dokunulmaz.

</details>

<details>
<summary><strong>PhotoGIMP'i kurduktan sonra kısayolları özelleştirebilir miyim?</strong></summary>

Elbette! PhotoGIMP yalnızca bir başlangıç noktası belirler. GIMP'te **Düzenle → Klavye Kısayolları** yolunu izleyerek istediğiniz kısayolu değiştirebilirsiniz.

</details>

<details>
<summary><strong>PhotoGIMP'i yeni bir sürüme nasıl güncellerim?</strong></summary>

En son sürümü indirip kurulum adımlarını yeniden uygulamanız yeterlidir — önceki PhotoGIMP yapılandırmasının üzerine yazılır.

</details>

---

## 🤝 Katkıda Bulunma

Bir hata mı buldunuz? Öneriniz mi var? Katkılarınızı bekliyoruz!

- **Hata bildirin**: [Bir issue açın](https://github.com/Diolinux/PhotoGIMP/issues)
- **Düzeltme gönderin**: [Bir pull request oluşturun](https://github.com/Diolinux/PhotoGIMP/pulls)
- **Çeviri yapın**: README'yi daha fazla dile çevirmemize yardım edin! [Çeviriler](#-çeviriler) bölümüne bakın.

---

## 🌍 Çeviriler

Bu README diğer dillerde de sunulmaktadır:

- 🇬🇧 [English (İngilizce)](../README.md)
- 🇮🇹 [Italiano (İtalyanca)](./README_it.md)
- 🇵🇱 [Polski (Lehçe)](./README_pl.md)
- 🇺🇦 [Українська (Ukraynaca)](./README_ua.md)
- 🇧🇷 [Português (Brezilya Portekizcesi)](./README_pt.md)
- 🇷🇺 [Русский (Rusça)](./README_ru.md)
- 🇪🇸 [Español (İspanyolca)](./README_es.md)
- 🇮🇱 [עברית (İbranice)](./README_he.md)
- 🇰🇷 [한국어 (Korece)](./README_ko.md)
- 🇨🇳 [简体中文 (Basitleştirilmiş Çince)](./README_zh.md)
- 🇨🇿 [Čeština (Çekçe)](./README_cs.md)

Dilinizi eklemek ister misiniz? Depoyu fork'layın, bir `docs/README_xx.md` dosyası oluşturun ve pull request gönderin!

---

## 🏆 Teşekkürler

- Bu proje, harika [GIMP](https://www.gimp.org/) ekibi olmadan mümkün olmazdı.
- Diolinux'un [YouTube](https://youtube.com/Diolinux) destekçilerinin tümüne ÇOK teşekkür ederiz.
- Açılış ekranı ve simgeler: [Adriel Filipe Design](https://bento.me/adrielfilipedesign).

---

## 👥 Katkıda Bulunanlar

<a align="center" href="https://github.com/Diolinux/PhotoGIMP/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Diolinux/PhotoGIMP" />
</a>

---

## 📄 Lisans

PhotoGIMP, [GNU Genel Kamu Lisansı v3.0](../LICENSE) kapsamında lisanslanmıştır.
