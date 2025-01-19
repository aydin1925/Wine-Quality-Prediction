# Şarap Kalitesi Tahmini

Bu depo, Portekiz "Vinho Verde" kırmızı şarabının kalitesini tahmin etmeye yönelik bir projeyi içermektedir. Proje, 11 kimyasal özelliği kullanarak şarap kalitesini tahmin etmek için makine öğrenimi tekniklerinden yararlanmaktadır.

## Projenin Amacı
Verilen veri setini analiz ederek şarabın kimyasal özelliklerine dayalı olarak kalitesini tahmin edebilecek bir model geliştirmek.

## Materyaller ve Yöntemler

### Veri Seti
Veri seti, Portekiz "Vinho Verde" şarabı hakkında bilgi içermektedir, özellikle kırmızı şarap çeşidi. Veri seti şu bilgileri içermektedir:
- **Özellikler (11 kimyasal özellik):**
  1. Fixed acidity
  2. Volatile acidity
  3. Citric acid
  4. Residual sugar
  5. Chlorides
  6. Free sulfur dioxide
  7. Total sulfur dioxide
  8. Density
  9. pH
  10. Sulfates
  11. Alcohol
- **Hedef:** Kalite puanı (0 ile 10 arasında değişmektedir)

**Veri Seti Özeti:**
- Toplam satır sayısı: 1599
- Toplam sütun sayısı: 12
- Eksik veri: Yok

### Kullanılan Makine Öğrenimi Modelleri
1. **Random Forest Classifier:** Başlangıç modeli olarak kullanıldı.
2. **Grid Search:** Model performansını artırmak için hiperparametre optimizasyonu yapıldı.

### Temel Adımlar
- Random Forest Classifier kullanılarak başlangıç modeli geliştirildi.
- Grid Search yöntemiyle hiperparametre optimizasyonu yapıldı.
- Veri setindeki sınıf dengesizlikleri giderildi.

## Sonuçlar
- **İlk Doğruluk Oranı:** %65.9
- **Grid Search Optimizasyonu Sonrası Doğruluk Oranı:** %68.4
- **Sınıf Dengesizlikleri Giderildikten Sonra Doğruluk Oranı:** %69.1

## Tartışma
Deneyler şunları göstermiştir:
1. Grid Search ile yapılan hiperparametre optimizasyonu model doğruluğunu önemli ölçüde artırmıştır.
2. Sınıf dengesizliklerinin giderilmesi modelin tahmin performansını daha da iyileştirmiştir.

## Nasıl Kullanılır
1. Bu depoyu klonlayın:
   ```bash
   git clone https://github.com/aydin1925/wine-quality-prediction
   ```
2. `Wine_quality_estimation.ipynb` notebook dosyasını açarak analizi görüntüleyin ve çalıştırın.

## Referanslar
1. Kaggle Red Wine Quality veri seti
2. Şanlıurfa Teknokent Makine Öğrenimi Eğitim Kaynakları
3. ChatGPT Yardımı

---

Projeye katkıda bulunmak için geliştirme önerileri yapabilir veya pull request gönderebilirsiniz!
