# iris-dataset-visualization
# Veri Yükleme ve Ön İşleme:
sklearn.datasets.load_iris() ile Iris veri setini yükler.
Özelliklere log-dönüştürme (np.log(0.1 + data)) uygulanarak veriler normalize edilir.
Veriler merkezlenir, yani her özellik kendi ortalamasından çıkarılır.

# Toplam Varyans Hesaplama:
Verinin toplam varyansı stot değişkenine atanarak hesaplanır.

# PCA Fonksiyonu:
PCA fonksiyonu, veriyi analiz etmek için kullanılır. Bu fonksiyon:
Kovaryans matrisini hesaplar.
Özdeğer ayrışımı (eigenvalue decomposition) ile kovaryans matrisini parçalar.
Özdeğerleri ve özvektörleri büyüklük sırasına göre sıralar.

# Scree Plot:
Ana bileşenlerin önemini görselleştirmek için bir scree plot oluşturulur. Bu grafik, her bir ana bileşenin toplam varyansa katkısını gösterir.

# Projeksiyon:
Veriler, ilk ana bileşene projekte edilir ve bu projeksiyon Z değişkeninde saklanır.

# Histogram Çizimi:
PCAplot fonksiyonu, her sınıf için ilk ana bileşen üzerine projekte edilen verilerin histogramını çizer.

# Ana Bileşen Formülü:
printformula fonksiyonu, ilk ana bileşenin formülünü oluşturan özvektörlerin katsayılarını ve özellikleri yazar.
