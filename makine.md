# Makinem: Baromak LUNA 1300 PRO

Bursa'daki Baromak firmasının ürettiği otomatik fırça zımpara makinesi. Masif, MDF ve kontrplaktan yapılmış kapı ve kapakların, özellikle CNC ile işlenmiş fugalı, rustik ve çıtalı modellerin kaba ve astar zımparasında kullanılıyor. Parça konveyörün üstünde makinenin içinden geçiyor, üstteki 6 fırça istasyonu zımparalıyor, çıkıştaki fırçalı temizleme istasyonu da tozunu alıp parçayı boyaya hazır hâle getiriyor.

## Teknik bilgiler (ilandan)

| Özellik | Değer |
|---|---|
| Toplam ağırlık | 3.730 kg |
| Ölçüler | 1970 × 4580 × 2300 mm |
| Toplam güç | 18 kW * |
| Voltaj | 380 V, 3 faz |
| Ürün genişliği | 10 – 1300 mm |
| Ürün uzunluğu | min. 400 mm, max. sınırsız |
| Ürün kalınlığı | 10 – 160 mm * |
| Konveyör hızı | max. 20 m/dk |

* İlanda toplam güç 18 kW, min. kalınlık 10 mm yazıyor. Baromak'ın kendi sayfasındaki teknik tabloda ise 14,5 kW ve 3 mm görünüyor. Hangisinin güncel olduğundan emin olamadım, föylerde ilandaki değerleri kullandım.

## Üreticinin sayfasından öğrendiklerim

- 6 adet birbirinden bağımsız, çift yönlü çalışan, osilasyonlu fırça istasyonu
- Dahili osilasyonlu cumba (kenar) zımpara istasyonu
- Her istasyonda 0,10 mm hassasiyetle baskı ayarı
- 10 inç dokunmatik panel (HMI)
- Reçete hafızası: her kapak modeli için ayarları isim verip kaydetme, tek tuşla çağırma
- **Uzaktan bağlantı:** üretici makineye 7/24 bağlanıp arıza tespiti ve eğitim yapabiliyor
- Lineer kızaklar için otomatik yağlama
- Bakım, temizlik ve zımpara değişimi için çekmeceli istasyonlar
- Her istasyonda, makine çalışırken zımparayı temizleyen hava üfleme sistemi
- Çıkışta fırçalı temizleme istasyonu ve 1 m'lik dahili çıkış konveyörü

## Varsayımlarım

Ne ilanda ne de üreticinin sayfasında makinenin emniyet donanımı (kaç acil stop var, kapaklarda kilit var mı, safety PLC mi emniyet rölesi mi kullanılıyor) yazıyor. Bu yüzden föyleri doldururken bu sınıf bir makinede olması gereken yapıyı varsaydım:

- Makine üstünde, girişte ve çıkışta acil stop butonları
- İstasyon çekmecelerinde ve bakım kapaklarında kilitli emniyet switchleri
- Bunları izleyen bir safety PLC (emniyet rölesi de olabilir)
- Fırça, osilasyon ve konveyör motorlarını süren inverterlerde STO girişi
- Normal kontrol tarafında bir PLC ve 10 inç HMI, üreticinin uzaktan bağlantısı da bu tarafa bir modem/router üzerinden geliyor

Gerçek makineyi görme imkânım olursa bu kısmı düzelteceğim.

Bu makineyi seçmemin bir sebebi de uzaktan bağlantı özelliğinin olması. Föylerdeki siber güvenlik kısmını havada bırakmadan gerçek bir bağlantı noktası üzerinden düşünebildim.

## Kaynaklar

- İlan: <https://twm.com.tr/tr/ilan/luna-1300-pro-firca-zimpara-makinesi>
- Üretici sayfası: <https://baromak.com.tr/urun-detay.html?id=luna-1300-pro>
