# Hafta 2: Python ile Ötegezegen (Exoplanet) Tespiti

![Python](https://img.shields.io/badge/PYTHON-3.12-007EC6?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/JUPYTER-NOTEBOOK-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Astronomy](https://img.shields.io/badge/ASTRONOMY-EXOPLANETS-yellow?style=for-the-badge)

> TESS ve Radyal Hız verileri kullanılarak simüle edilmiş bir ötegezegen sisteminin (HD 1234 b) modellenmesi ve analizi.

##  Bu Hafta Neler Yapıldı?
Bu hafta, astrofizikte ötegezegen keşfi için en çok kullanılan iki ana yöntemi Python yardımıyla uygulamalı olarak inceledik ve modellendirdik:

1. **Geçiş (Transit) Yöntemi ve Işık Eğrileri:**
   * TESS (Transiting Exoplanet Survey Satellite) verilerine benzer şekilde hazırlanan `HD 1234 Light Curve.csv` veri seti yüklendi.
   * `batman` kütüphanesi kullanılarak gezegenin yıldız önünden geçişi (transit) modellendi.
   * Gezegenin yarıçapı ($R$), yörünge periyodu ($P$) ve eğikliği ($inc$) gibi temel parametreler manuel olarak (deneme-yanılma yoluyla) veriyle eşleştirildi.

2. **Dikey Hız (Radial Velocity - RV) Yöntemi:**
   * `HD 1234 RVs.csv` veri seti üzerinden yıldızın gezegen çekimiyle yaptığı Doppler kaymaları incelendi.
   * Kepler yasaları ve eliptik yörünge denklemleri kullanılarak gezegenin kütlesi ($M$) ve yörünge özellikleri karakterize edildi.

3. **Gezegen Kompozisyonu Analizi:**
   * Elde edilen kütle ve yarıçap değerleri kütle-yarıçap (Mass-Radius) teorik eğrileriyle karşılaştırılarak gezegenin yapısının kaya/demir karışımı (kayasal ötegezegen) olduğu belirlendi.

## Dosya Yapısı
* `Intro2Astro Exoplanet Detection Methods.ipynb`: Çalışmanın adım adım gerçekleştirildiği Jupyter Notebook dosyası.
* `HD 1234 Light Curve.csv`: Simüle edilmiş geçiş ışık eğrisi verisi.
* `HD 1234 RVs.csv`: Simüle edilmiş dikey hız verisi.