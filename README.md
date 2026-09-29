<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=soft&color=0:FCAF01,50:FE2C6B,100:FC05AC&height=160&section=header&text=Grave&fontSize=60&fontColor=FFFFFF&fontAlignY=42&desc=Spigot%20%2F%20Paper%20%E2%80%A2%201.8%20%E2%86%92%201.21.11&descSize=15&descAlignY=72&animation=fadeIn" alt="Grave" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/coslant/Grave/releases/latest"><img src="https://img.shields.io/github/v/release/coslant/Grave?style=for-the-badge&label=%C4%B0ndir&color=FE2C6B&logo=github" alt="Download" /></a>
  <a href="https://discord.gg/forges"><img src="https://img.shields.io/badge/Discord-Forges%20Studio-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord: Forges Studio" /></a>
</p>

<p align="center">
  <a href="https://github.com/coslant/Grave/actions/workflows/build.yml"><img src="https://img.shields.io/github/actions/workflow/status/coslant/Grave/build.yml?branch=main&style=flat-square&label=build" alt="Build" /></a>
  <img src="https://img.shields.io/badge/Minecraft-1.8%20%E2%86%92%201.21.11-FCAF01?style=flat-square" alt="Minecraft 1.8 - 1.21.11" />
  <img src="https://img.shields.io/badge/Spigot%20%7C%20Paper-FE9808?style=flat-square" alt="Spigot | Paper" />
  <img src="https://img.shields.io/badge/Java-8-FD6C29?style=flat-square&logo=openjdk&logoColor=white" alt="Java 8" />
  <a href="LICENSE"><img src="https://img.shields.io/github/license/coslant/Grave?style=flat-square&color=FB0C9E&label=lisans" alt="License" /></a>
</p>

<p align="center">
  <b>Ölünce eşyalar mezarda durur, üzerinde hologram ve geri sayım.</b>
  <br>
  <sub><kbd>EN</kbd> Keeps your items in a grave with a hologram and countdown when you die.</sub>
</p>

Ölünce eşyaların yere saçılmak yerine bir mezarda saklanır. Mezarın üstünde hologram ve geri sayım durur.
Tek jar **1.8 – 1.21.11** arası çalışır.

## ✨ Özellikler

- ⚰️ Ölüm yerinde sandık + üstünde çok satırlı **hologram** ve canlı **geri sayım**
- 💾 **Mezarlar `graves.yml` dosyasında saklanır** — sunucu yeniden başlasa bile eşyaların durur
- ✨ **Tecrübe de saklanır**, mezarı açınca geri verilir
- 🔒 Mezar başkaları tarafından kırılamaz, patlamayla yok edilemez
- 👥 Sadece sahibi ya da herkes açabilsin — senin seçimin
- 📍 `/grave list` ile mezarlarının yerini ve kalan süresini gör
- ⏱️ Süre dolunca eşyalar yere dökülür ya da doğrudan sahibine iade edilir
- 🕳️ Boşluğa, lavın içine ya da blok içine düşersen mezar güvenli bir noktaya kurulur
- 🔢 Oyuncu başına mezar limiti

## 📥 Kurulum

1. [Releases](https://github.com/coslant/Grave/releases/latest) sayfasından `Grave.jar` dosyasını indir.
2. Sunucunun `plugins/` klasörüne at.
3. Sunucuyu yeniden başlat.
4. `plugins/Grave/config.yml` dosyasından süreyi ve hologramı düzenle.

## 🎮 Komutlar

| Komut | Açıklama | Yetki |
|-------|----------|-------|
| `/grave list` | Mezarlarını ve kalan sürelerini listeler | herkes |
| `/grave reload` | Ayarları yeniden yükler | `grave.reload` |

**Alias:** `/mezar`

## 🔑 Yetkiler

| Yetki | Açıklama | Varsayılan |
|-------|----------|------------|
| `grave.use` | Ölünce mezar oluşur | herkes |
| `grave.open.others` | Başkalarının mezarlarını açabilir | op |
| `grave.reload` | Configi yeniden yükler | op |

## ⚙️ Ayarlar (config.yml)

| Anahtar | Açıklama |
|---------|----------|
| `duration` | Mezar kaç saniye durur |
| `keep-experience` | Tecrübe de saklansın mı |
| `only-owner` | Sadece sahibi açabilsin mi |
| `protect` | Mezar kırılmaya ve patlamaya karşı korunsun mu |
| `place-chest` / `chest-material` | Görsel sandık konsun mu, hangi blok |
| `max-graves-per-player` | Oyuncu başına mezar limiti (0 = sınırsız) |
| `return-to-owner-on-expire` | Süre dolunca eşyalar sahibine mi verilsin |
| `hologram.lines` | Hologram satırları |
| `hologram.height` / `line-spacing` | Hologram yüksekliği ve satır aralığı |

### Yer tutucular

`%player%` · `%player_in%` (ilgi ekli: *coslant'ın*) · `%time%` · `%items%` · `%xp%` · `%x%` `%y%` `%z%` `%world%`

## 🛠️ Derleme

```bash
mvn clean package
```

Çıktı: `target/Grave.jar`

> 1.8 uyumluluğu için Java 8 hedefiyle derlenir. En sorunsuz derleme **JDK 8, 11 veya 17** iledir.

Her push'ta [GitHub Actions](https://github.com/coslant/Grave/actions/workflows/build.yml) projeyi otomatik derler; etiketlenen sürümler (`v*`) jar'ıyla birlikte [Releases](https://github.com/coslant/Grave/releases) sayfasında yayınlanır.

## 💬 Destek

- 🐛 Hata bildirimi ve öneriler için [Issues](https://github.com/coslant/Grave/issues) sekmesini kullan.
- 💬 Sorular ve destek için [Forges Studio Discord](https://discord.gg/forges) sunucusuna katıl.

## 📄 Lisans

[MIT](LICENSE) — dilediğin gibi kullan, değiştir, dağıt.

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:FCAF01,50:FE2C6B,100:FC05AC&height=4&section=footer" width="100%" alt="" />
  <br>
  <sub>🔥 <a href="https://github.com/coslant">coslant</a> tarafından geliştirildi · <a href="https://discord.gg/forges">Forges Studio</a></sub>
</p>
