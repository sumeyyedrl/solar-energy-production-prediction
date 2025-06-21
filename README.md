# ☀️ Güneş Enerjisi Tahmin Projesi

Bu proje, Python ile zaman serisi modelleme (SARIMAX) ve makine öğrenmesi (XGBoost) kullanarak güneş enerjisi üretimini tahmin etmeye yönelik geliştirilmiştir.
Güneş enerjisi lisanslı üretimi ve güneş enerjisi lisanslı kurulu gücü EPİAŞ Şeffaflık tarafından çekilmiş olup, kullanıcı adı ve şifre bilgisine ihtiyaç duyulmaktadır. Bu [linkten](https://seffaflik.epias.com.tr/home) üye olabilirsiniz veya ilgili veriler elde edildikten sonra güneş_enerji_veriler klasörüne yüklendiğinden direkt kullanabilirsiniz. Böylece API ile veri çekilen ilgili kod parçalarının çalıştırılmasına gerek kalmadan proje çalıştırılabilir ve test edilebilir.

## 📁 Proje İçeriği

- Zaman serisi analizi (ADF testi, SARIMAX)
- XGBoost regresyon modeli ve hiperparametre optimizasyonu (GridSearchCV)
- Görselleştirme ve model performans analizi
- API ile veri çekimi (requests, requests_cache, retry_requests)

## 🚀 Kurulum ve Kullanım

### 1. Repozitoyu Klonla
```bash
git clone https://github.com/sumeyyedrl/solar-energy-production-prediction.git
cd solar-energy-production-prediction
```

### 2. Sanal Ortam Oluştur (Opsiyonel ama önerilir)
```bash
python -m venv venv  #Windows
venv\Scripts\activate  #MacOS / Linux
source venv/bin/activate
```

### 3. Gerekli Kütüphaneleri Yükle
```bash
pip install -r requirements.txt
```

### Dikkat!
Projede kullanılan ve API yoluyla elde edilen büyük hacimli veriler zaman tasarrufu adına güneş_enerji_veriler klasöründe hazır olarak sunulmuştur. Direkt klasördeki veriler import edilerek de proje çalıştırılabilir. Bu veriler içerisindeki weather.zip ayıklanıp içerisindeki weather.csv dosyası, güneş_enerji_veriler klasörünün altına kopyalanmalıdır.
