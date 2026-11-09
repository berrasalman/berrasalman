<!--
  BERRA SALMAN | YBS — Tek dosyalık GitHub profil README
  Bu sürümde ./assets/ altında dosya aranmaz.
  Banner: capsule-render adlı harici görsel servisi.
  Yılan animasyonu: Platane/snk projesinin DEMO görseli (Berra'nın katkıları değildir).
  Berra'nın kendi katkı grafiği için ayrıca GitHub Actions gerekir.
-->

<div align="center">

  <img width="100%" alt="Berra SALMAN | YBS - Tiyatro, Teknoloji ve Yaratıcılık" src="https://capsule-render.vercel.app/api?type=waving&color=0:111827,45:5B21B6,100:059669&height=240&section=header&text=Berra%20SALMAN%20%7C%20YBS&fontColor=FFFFFF&fontSize=42&fontAlignY=38&desc=TECH%20%E2%80%A2%20THEATRE%20%E2%80%A2%20CREATIVITY&descSize=16&descAlignY=62&animation=fadeIn" />

  <h2>Merhaba, ben Berra! 👋</h2>

  <p>
    🎓 <b>Yönetim Bilişim Sistemleri</b> öğrencisi<br/>
    💻 Teknoloji ve yazılım dünyasını keşfediyorum<br/>
    🎭 Tiyatro ve sahne sanatlarıyla ilgileniyorum
  </p>

  <p>
    <img src="https://img.shields.io/badge/YBS-Y%C3%B6netim%20Bili%C5%9Fim%20Sistemleri-6D28D9?style=for-the-badge" alt="YBS" />
    <img src="https://img.shields.io/badge/Creative-Tiyatro-DB2777?style=for-the-badge" alt="Tiyatro" />
    <img src="https://img.shields.io/badge/Arcade-Snake%20Game-059669?style=for-the-badge" alt="Snake Game" />
  </p>

  <img alt="Yaratıcılık temalı hareketli yazı" src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&pause=1200&color=AD8AFF&center=true&vCenter=true&width=620&lines=Kodda+mantik%2C+sahnede+hikaye.;Learn.+Create.+Express.+Grow." />

</div>

---

### ✨ Biraz benden

Yönetim Bilişim Sistemleri alanında öğrenmeye ve üretmeye devam ediyorum. Teknolojinin çözüm üreten yönünü, tiyatronun ise anlatım ve yaratıcılık tarafını seviyorum. Bazen bir algoritma, bazen bir sahne: İkisi de yeni bir şey ortaya koymanın farklı yolları.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>💻 Teknoloji & YBS</h3>
      Yazılım • Problem çözme • Dijital dönüşüm • Yeni fikirler
    </td>
    <td width="50%" valign="top">
      <h3>🎭 Tiyatro & Sahne</h3>
      Hikâye anlatımı • Yaratıcılık • İfade • Takım çalışması
    </td>
  </tr>
</table>

---

### 🐍 Snake Zone

<div align="center">

  <h3>🎮 RETRO SNAKE</h3>
  <p>🟩 🟩 🟩 🟩 🟢 &nbsp; 🍎</p>
  <sub>Biraz nostalji, biraz eğlence, bolca yaratıcılık.</sub>

</div>

```
╔══════════════════════════════════╗
║  S N A K E   Z O N E       🍎     ║
║                                  ║
║      🟩🟩🟩🟩🟩🟢                  ║
║                                  ║
║        YBS × THEATRE × CODE      ║
╚══════════════════════════════════╝
```

Klasik yılan oyununun mantığı basit: Yemleri topla, yılanı büyüt, duvara veya kendi kuyruğuna çarpmadan devam et! GitHub README doğrudan JavaScript çalıştıramadığı için burada **oynanabilir bir uygulama yerine tematik bir tanıtım** bulunuyor.

[🎮 Açık kaynaklı Snake demosunu oyna](https://opengames-dev.github.io/snake/) · [🐍 Snake animasyonu nasıl üretilir?](https://github.com/Platane/snk)

---

### 🌿 Hareketli yılan animasyonu

<div align="center">
  <img width="100%" alt="Örnek hareketli GitHub katkı yılanı (Platane/snk demosu)" src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" />
  <br/>
  <sub>Bu, Platane/snk projesinin örnek animasyonudur; Berra'nın kişisel katkı grafiği değildir.</sub>
</div>

<details>
  <summary><b>⚙️ Kendi GitHub katkılarımla hareket eden yılan nasıl yapılır?</b></summary>

  Profil deposunda `.github/workflows/snake.yml` oluşturup aşağıdaki kodu ekle. Bu işlem README'den ayrı, tek seferlik bir GitHub Actions kurulumu gerektirir.

  ```yaml
  name: Generate contribution snake

  on:
    workflow_dispatch:
    schedule:
      - cron: '0 6 * * *'

  permissions:
    contents: write

  jobs:
    build:
      runs-on: ubuntu-latest
      steps:
        - uses: Platane/snk/svg-only@v3
          with:
            github_user_name: ${{ github.repository_owner }}
            outputs: |
              dist/snake.svg?color_snake=%2386efac
              dist/snake-dark.svg?palette=github-dark&color_snake=%23a78bfa
        - uses: crazy-max/ghaction-github-pages@v4
          with:
            target_branch: output
            build_dir: dist
          env:
            GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  ```

  Actions > Generate contribution snake > Run workflow kısmından çalıştır. Başarılı olunca üstteki DEMO görselinin URL'sini kendi kullanıcı adına göre değiştir:

  `https://raw.githubusercontent.com/KULLANICI_ADI/KULLANICI_ADI/output/snake-dark.svg`

  > GitHub Actions izni gerekiyorsa Settings → Actions → General → Workflow permissions bölümünü kontrol et.
</details>

---

### 🎭 Sahne arkasında, kodun başında

> **“Kodda mantık, sahnede hikâye. Her ikisinde de yaratıcılık.”**

Yeni şeyler öğrenmeyi, farklı fikirleri bir araya getirmeyi ve üretmeye devam etmeyi seviyorum. Teknolojiyle sahnenin buluştuğu yerlerde daha çok şey keşfetmek istiyorum.

<div align="center">
  <h3>Berra SALMAN</h3>
  <b>Yönetim Bilişim Sistemleri • Teknoloji • Tiyatro</b>
  <p>💜 Learn · Create · Express · Grow 🐍</p>
  <img width="100%" alt="Sayfa sonu" src="https://capsule-render.vercel.app/api?type=waving&color=0:111827,45:5B21B6,100:059669&height=110&section=footer" />
</div>
