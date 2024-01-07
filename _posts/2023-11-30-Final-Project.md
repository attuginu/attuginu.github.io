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
   - TAS [<u>(Le Bas et al., 1986)</u>](https://doi.org/10.1093/petrology/27.3.745)
   - K-Series [<u>(Gill, 1981)</u>](https://doi.org/10.1007/978-3-642-68012-0)
   - Tholeiitic vs. Calc-Alkaline [<u>(Miyashiro, 1974</u>)](https://doi.org/10.2475/ajs.274.4.321)
   - Tholeiitic vs. Calc-Alkaline [<u>(Irvine and Baragar, 1971</u>)](https://doi.org/10.1139/e71-055.1)
   - Harker [<u>(Harker, 1909</u>)](https://archive.org/details/naturalhistoryof00harkuoft/mode/2up)
   - Spidergram REE [<u>(Sun and McDonough, 1989</u>)](https://doi.org/10.1144/GSL.SP.1989.042.01.19)
   - Spidergram Trace Element [<u>(Pearce, 1983</u>)](https://www.researchgate.net/publication/247434731_Role_of_the_sub-continental_lithosphere_in_magma_genesis_at_active_continental_margin)
2. Analisis Komputasi Geosains
   -  Principal Component Analysis
   -  K-Means Clustering 
   -  Gaussian Mixing Model.  

# Data
<p style="text-align:justify">Data yang digunakan merupakan data yang berasal dari database GeoRoc oleh <a href="https://georoc.mpch-mainz.gwdg.de/georoc/"> <u>Digis Team</u></a>. Pada database didapatkan tiga dokumen, yakni “Luzon Arc”, “Sulawesi Arc”, dan “Halmahera Arc” yang berasal dari kategori “Convergent Margin”. Ketiga dokumen ini berisi total 2987 sampel data geokimia yang terdiri dari batuan vulkanik, beku, sedimen, dan metamorf yang tersebar sepanjang area Sulawesi, Halmahera, Filipina, dan Kalimantan. Ketiga file memiliki informasi asal data, unsur mayor, unsur jejak, dan isotop dari setiap sampel. Dataset ini nantinya akan disaring sehingga dapat diketahui data yang dapat digunakan pada analisis berikutnya.</p>
<p style="text-align:justify">Data akan difilter sehingga hanya berisi parameter yang digunakan. proses ini menggunakan python library: pandas. Dataset ini yang kemudian akan digunakan sepanjang penelitian.</p>

# Output
