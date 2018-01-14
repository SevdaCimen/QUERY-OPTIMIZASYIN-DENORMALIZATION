# QUERY OPTIMIZASYON-DENORMALIZATION
  
  
  
  ![query](https://user-images.githubusercontent.com/26030084/34914572-42f0e61e-f926-11e7-917f-d433912a74b0.jpg)

Optimizer ya da diger isimleri ile query optimizer veya cost based optimizer bir veritabanı
parc¸asıdır ve SQL ifadelerinin nasıl kos¸ulması gerekti˘ginin
yolunun c¸ıkartılmasını sa˘glar. B¨ut¨un SQL ifadeleri optimizer’ı
kullanmaktadır. ”Cost” adı verilen bir miktar hesaplanmakta
ve SQL ifadeleri bu y¨onden kos¸turulmaktadır.Sorgunun
c¸alıs¸tırılması planını hazırlar. Sorgulama planlayıcısı ve
optimize edicisi zor olan du¨s¸u¨nme is¸ini yapar. O¨ nce basit
optimizasyonlar uygular (5*10’u 50 olarak sadeles¸tirmek gibi
daha iyi performansla sonuc¸lanan iyiles¸tirmeler). Sonra farklı
optimizasyonları olan farklı ”sorgulama planlarına” bakar,
her bir sorgulama planının ilgili tablolardaki satırlara g¨ore
maliyetini (CPU ve s¨ure) tahmin eder, sonra en iyi planı
alır ve sonraki adıma gec¸irir. Basit bir SELECT sorgusu
ic¸in sadece bir plan vardır ve maliyetsiz (zero cost) olarak
tanımlanır. Karmas¸ık sorgular ic¸in 3 as¸amalı bir optimizasyon
yapılır:



DENORMALIZATION
Önce normalize et, eger performans problemi var ise denormalize işlemi uygula” dır. Denormalizasyon işleminin kesin
kuralları yoktur ve veritabanı tasarımcısının sorguların yavaşlamasına karşın bulduğu cözümler olarak düşünülebilir.
Denormalizasyon işlemi performans kazanımları düşünülüp sadece gerekli tablolara uygulanması yeterli bir işlemdir.

![denormalizasyon](https://user-images.githubusercontent.com/26030084/34914603-b8826c72-f926-11e7-89d7-b7a9892e61a3.PNG)
