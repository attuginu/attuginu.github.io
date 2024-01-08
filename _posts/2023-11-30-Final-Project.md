---
layout: post
title: "Application of Computational Geoscience for Geochemical Characterization of Subduction Zone Volcanic Rocks"
subtitle: "My Final Project as Undergraduate Student"
background: '/img/posts/2023-11-30-Final-Project/bg.jpg'
---

# Pendahuluan
<p style="text-align:justify">Tugas akhir ini berfokus pada karakterisasi data geokimia di tiga busur kepulauan: Busur Sangihe, Busur Halmahera, dan Busur Busur Filipina Timur. Karakterisasi yang dilakukan menggunakan plot geokimia dan analisis komputasi"</p>  

# Metode
1. Diagram Geokimia
   - TAS [<u>(Bas et al., 1986)</u>](https://doi.org/10.1093/petrology/27.3.745)
   - K-Series [<u>(Gill, 1981)</u>](https://doi.org/10.1007/978-3-642-68012-0)
   - Tholeiitic vs. Calc-Alkaline [<u>(Miyashiro, 1974</u>)](https://doi.org/10.2475/ajs.274.4.321) dan [<u>(Irvine and Baragar, 1971</u>)](https://doi.org/10.1139/e71-055.1)
   - Harker [<u>(Harker, 1909</u>)](https://archive.org/details/naturalhistoryof00harkuoft/mode/2up)
   - Spidergram REE [<u>(Sun and McDonough, 1989</u>)](https://doi.org/10.1144/GSL.SP.1989.042.01.19)
   - Spidergram Trace Element [<u>(Pearce, 1983</u>)](https://www.researchgate.net/publication/247434731_Role_of_the_sub-continental_lithosphere_in_magma_genesis_at_active_continental_margin)
2. Analisis Komputasi Geosains
   -  Principal Component Analysis (PCA)
   -  K-Means Clustering (KMC)
   -  Gaussian Mixing Model (GMM)  

# Data
<p style="text-align:justify">Data yang digunakan merupakan data yang berasal dari database GeoRoc oleh <a href="https://georoc.mpch-mainz.gwdg.de/georoc/"> <u>Digis Team</u></a>. Pada database didapatkan tiga dokumen, yakni “Luzon Arc”, “Sulawesi Arc”, dan “Halmahera Arc” yang berasal dari kategori “Convergent Margin”. Ketiga dokumen ini berisi total 2987 sampel data geokimia yang terdiri dari batuan vulkanik, beku, sedimen, dan metamorf yang tersebar sepanjang area Sulawesi, Halmahera, Filipina, dan Kalimantan. Ketiga file memiliki informasi asal data, unsur mayor, unsur jejak, dan isotop dari setiap sampel. Dataset ini nantinya akan disaring sehingga dapat diketahui data yang dapat digunakan pada analisis berikutnya.</p>
<p style="text-align:justify">Data akan difilter sehingga hanya berisi parameter yang digunakan. proses ini menggunakan python library: pandas. Dataset ini yang kemudian akan digunakan untuk penelitian.</p>

# Output
## - Diagram Geokimia 
Gambar di bawah menunjukan karakteristik geokimia menggunakan diagram geokimia
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/TAS.jpg"
         alt="Diagram TAS">
    <span class="caption text-muted">Diagram TAS (Bas et al., 1986) menunjukan batuan vulkanik yang terbentuk dan 
terdapat garis pembeda alkali vs. subalkali (Irvine & Baragar, 1971).</span>
</figure>
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/k-series.png"
         alt="Diagram K-series">
    <span class="caption text-muted">Diagram Gill (1981) menunjukan bahwa terdapat dua seri-K pada batuan 
vulkanik daerah penelitian: medium-K dan high-K.</span>
</figure>
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/miyashiro.png"
         alt="Tholeiitic vs. Calc-Alkaline">
    <span class="caption text-muted">Diagram Miyashiro (1979) menunjukan bahwa seluruh batuan vulkanik termasuk pada seri calc-alkaline. Terdapat sebagian kecil anomali yang menunjukan seri tholeiitic. </span>
</figure>
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/afm.png"
         alt="Tholeiitic vs. Calc-Alkaline">
    <span class="caption text-muted">Diagram AFM (Irvine & Baragar, 1971) menunjukan bahwa seluruh batuan vulkanik termasuk seri calc-alkaline.</span>
</figure>
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/harker_mayor.png"
         alt="Harker Mayor Element">
    <span class="caption text-muted">Diagram Harker (1909) unsur mayor batuan vulkanik daerah penelitian</span>
</figure>
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/harker_trace.png"
         alt="Harker Trace Element">
    <span class="caption text-muted">Diagram Harker (1909) unsur jejak batuan vulkanik daerah penelitian</span>
</figure>
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/spider.png"
         alt="Spidergram">
    <span class="caption text-muted">Diagram spider unsur jejak dan REE daerah penelitian</span>
</figure>

## - Komputasi Geosains
### 1. Principal Component Analysis
- unsur mayor
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/major_pca.png"
         alt="PCA Unsur Mayor">
    <span class="caption text-muted">Biplot dari principal component 1 dan principal component 2 pada unsur mayor daerah penelitian. dihadirkan pula vector loading dari variabel awal.</span>
</figure>
- unsur jejak
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/trace_pca.png"
         alt="PCA Unsur Jejak">
    <span class="caption text-muted">Biplot dari principal component 1, principal component 2, dan principal component 3 pada unsur jejak daerah penelitian. dihadirkan pula vector loading dari variabel awal</span>
</figure>

### 2. Analisis Klaster
- unsur mayor
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/major_kmc_gmm.png"
         alt="KMC dan GMM Unsur Mayor">
    <span class="caption text-muted">Biplot dari analisis k-means clustering (atas) dan gaussian mixture model (bawah).</span>
</figure>
- unsur jejak
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/trace_kmc.png"
         alt="KMC Unsur Jejak">
    <span class="caption text-muted">Biplot k-means clustering pada rasio unsur jejak</span>
</figure>
<figure>
    <img src="/img/posts/2023-11-30-Final-Project/trace_gmm.png"
         alt="GMM Unsur Jejak">
    <span class="caption text-muted">Biplot Gaussian Mixture Model pada rasio unsur jejak</span>
</figure>