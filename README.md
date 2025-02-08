# 🔍 Morfolojik Operasyonlar ve Kontur Tanıma Algoritmaları
Bu projede, bir el görüntüsü üzerinde çeşitli görüntü işleme teknikleri uygulanmıştır. Gürültü azaltma, eşikleme, morfolojik işlemler, mesafe dönüşümü ve Watershed algoritması gibi yöntemler kullanılarak elin sınırları belirlenmiş ve konturlar çizilmiştir. Son olarak, görüntü yansıtılarak ekranda gösterilmiştir.
## 🛠 Kullanılan Teknolojiler

🐍 Python → Görüntü işleme ve veri analizi.

🖼 OpenCV → Görüntü işleme ve filtreleme işlemleri.

🔢 NumPy → Matris işlemleri ve veri yönetimi.

📊 Matplotlib → Görselleştirme ve grafik çizimi.

## 📌 Kullanılan Algoritmalar ve Yöntemler

🔗 Median Blur - Gürültü Azaltma
Görüntüdeki tuz-biber (salt & pepper) gürültüsünü azaltmak için kullanılır. Ortadaki piksel değeri kullanılarak komşu piksellerle yumuşatma işlemi yapılır.

🔗 Gri Tonlama Dönüşümü (Grayscale Conversion)
Renkli görüntü gri tonlamaya çevrilerek işlem süreci hızlandırılır ve algoritmalar için uygun hale getirilir.

🔗 Binary Thresholding - İkili Eşikleme
Pikseller belirlenen 160 eşik değeri ile siyah-beyaz olarak ayrılır. Beyaz alanlar nesneyi, siyah alanlar ise arka planı temsil eder.

🔗 Açma (Opening) - Gürültü Temizleme

Küçük boyuttaki gürültüleri ortadan kaldırarak nesnenin daha belirgin hale gelmesini sağlar.

🔗 Dilatasyon (Dilation) - Nesne Sınırlarını Genişletme

Nesne sınırları genişletilerek boşluklar kapatılır ve daha belirgin hale getirilir.

🔗 Mesafe Dönüşümü (Distance Transform)

Nesnelerin merkez noktaları belirlenerek, watershed algoritması için ön bilgi sağlanır.

🔗 Watershed Algoritması - Nesne Sınırlarını Belirleme

Görüntü üzerindeki nesnelerin sınırlarını watershed segmentation yöntemiyle belirler.

🔗 Connected Components Analysis

Görüntüdeki farklı nesneleri etiketleyerek belirli bölgelere ayırır.

🔗 Kontur Bulma (Contour Detection)

Görüntüdeki dış ve iç sınırları belirler.

RETR_CCOMP: İç içe geçmiş konturları hiyerarşik olarak bulur.

CHAIN_APPROX_SIMPLE: Kontur noktalarını sıkıştırarak gereksiz verileri kaldırır.

🔗 Kontur Çizme (Drawing Contours)

Bulunan dış konturlar, yeşil renkle görüntü üzerine çizilir.

🔗 Görüntü Yansıtma (Flip - Mirroring the Image)

Görüntü yatay eksende çevrilerek aynalanır.

🔗 Sonuçları Görselleştirme

display() fonksiyonu kullanılarak her adımın sonucu matplotlib ile ekranda gösterilir.
