# Heartlytics
Heartlytics: Kalp Hastalığı Veri Analizi ve Tahmin Modeli  Bu repo, kalp hastalığı veri seti üzerinde kapsamlı bir analiz ve tahmin çalışması sunar. Veri temizleme, eksik değer doldurma, görselleştirme ve lojistik regresyon tabanlı makine öğrenimi modeli oluşturma gibi adımları içerir. 

# Kalp Hastalığı Veri Analizi ve Modelleme

Bu repo, kalp hastalığı veri setinin temizlenmesi, analizi ve lojistik regresyon tabanlı bir model ile tahmin yapılmasını içerir. Veriler üzerinde eksik değer doldurma, görselleştirme ve makine öğrenimi teknikleri uygulanmıştır.

## Proje İçeriği

### 1. Veri Setleri

- **`data.csv`**: Ham veri seti.
- **`cleaned_data.csv`**: Eksik değerlerin doldurulması ve temel veri temizleme işlemleri yapılmış veri seti.
- **`cleaned_data_fixed.csv`**: İsimlendirme ve sütun düzenlemeleri yapılmış, nihai temiz veri seti.

### 2. Veri İşleme Adımları

#### Eksik Değer Doldurma:
- **Sayısal sütunlar:** Medyan değer kullanılarak doldurulmuştur.
- **Kategorik sütunlar:** Mod (en sık görülen değer) kullanılarak doldurulmuştur.

#### Veri Temizleme:
- Tüm sütun isimlerindeki fazladan boşluklar kaldırılmıştır.

### 3. Çıktılar ve Analizler
- Temizlenen veri seti analiz edilerek demografik ve hastalık ilişkileri ortaya konmuştur.
- Görselleştirme araçları ile yaş grupları, cinsiyet ve hastalık durumu gibi faktörler değerlendirilmiştir.

### 4. Makine Öğrenimi
- **Lojistik Regresyon:** Hastalık tahmini için bir model oluşturulmuş ve doğruluk oranı hesaplanmıştır.
- **ROC-AUC Analizi:** Modelin performansı değerlendirilmiştir.

## Kullanım

### Gereksinimler
Projeyi çalıştırmadan önce aşağıdaki kütüphanelerin yüklü olduğundan emin olun:

- **Python 3.7+**
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

### Veri Setlerini İnceleme
Veri setlerini bu repo üzerinden indirebilir ve inceleyebilirsiniz:

1. `data.csv`: Ham veri setiyle başlayın.
2. `cleaned_data.csv`: Temizlenmiş veri setini kullanarak temel analiz yapabilirsiniz.
3. `cleaned_data_fixed.csv`: Sütun isimleri düzenlenmiş nihai veri setidir.

### Çalıştırma
Bu proje için kodları çalıştırmadan önce `cleaned_data_fixed.csv` dosyasını uygun bir dizine koyun ve aşağıdaki adımları takip edin:

1. **Veri Setini Yükleyin:**
   ```python
   import pandas as pd
   data = pd.read_csv('cleaned_data_fixed.csv')
   ```
2. **Analiz ve Görselleştirme:** Kod parçacıklarını kullanarak veriyi analiz edin ve görselleştirin.
3. **Model Eğitimi ve Test:** Makine öğrenimi kodunu çalıştırarak model performansını değerlendirin.



