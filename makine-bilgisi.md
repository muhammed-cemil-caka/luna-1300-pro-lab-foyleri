# Makine Bilgisi: Baromak LUNA 1300 PRO

Bursa'daki Baromak firmasının ürettiği otomatik fırça zımpara makinesi. Masif, MDF ve kontrplaktan yapılmış kapı ve kapakların, özellikle CNC ile işlenmiş fugalı, rustik ve çıtalı modellerin kaba ve astar zımparasında kullanılıyor. Parça konveyörün üstünde makinenin içinden geçiyor, 6 fırça istasyonu ve bir cumba istasyonu zımparalıyor, çıkıştaki fırçalı temizleme istasyonu da tozunu alıp parçayı boyaya hazır hâle getiriyor.

**Teknik bilgiler**

| Özellik | Değer |
|---|---|
| Toplam ağırlık | 3.730 kg |
| Ölçüler | 1970 × 4580 × 2300 mm |
| Toplam güç | 18 kW (üretici sayfasında 14,5 kW) |
| Besleme | 380 V, 3 faz |
| Ürün genişliği | 10 – 1300 mm |
| Ürün uzunluğu | en az 400 mm, üst sınır yok |
| Ürün kalınlığı | 10 – 160 mm (üretici sayfasında en az 3 mm) |
| Konveyör hızı | en fazla 20 m/dk |

İlan ile üreticinin sayfası arasında güç ve minimum kalınlık değerleri farklı. Hangisinin güncel olduğunu bilmediğim için ikisini de yazdım; föylerdeki hesaplar bu değerlere bağlı değil.

## Üreticinin sayfasından öğrendiklerim

- 6 adet birbirinden bağımsız, çift yönlü çalışan, osilasyonlu fırça istasyonu
- Dahili osilasyonlu cumba (kenar) zımpara istasyonu
- Her istasyonda 0,10 mm hassasiyetle baskı ayarı
- 10 inç dokunmatik panel, reçete hafızası (model adıyla kaydetme, tek tuşla çağırma)
- **Uzaktan bağlantı:** üretici makineye 7/24 bağlanıp arıza tespiti ve eğitim yapabiliyor
- Lineer kızaklar için otomatik yağlama
- Bakım, temizlik ve zımpara değişimi için çekmeceli istasyonlar
- Her istasyonda çalışma sırasında zımparayı temizleyen hava üfleme
- Çıkışta fırçalı temizleme istasyonu ve 1 m'lik çıkış konveyörü

## Varsayımlarım

İlanda da üreticinin sayfasında da makinenin emniyet donanımı (kaç acil stop olduğu, kapaklarda kilit olup olmadığı, safety PLC mi emniyet rölesi mi kullanıldığı) yazmıyor. Föyleri hazırlarken bu sınıf bir makinede bulunması gereken yapıyı varsaydım:

- Makine üstünde, girişte ve çıkışta acil stop butonları
- İstasyon çekmecelerinde ve bakım kapaklarında kilitli emniyet switchleri
- Bunları izleyen bir safety PLC
- Fırça, osilasyon ve konveyör motorlarını süren inverterlerde STO girişi
- Normal kontrol tarafında bir PLC ve 10 inç HMI; üreticinin uzaktan bağlantısı bu tarafa bir modem üzerinden geliyor

Makineyi yerinde görme fırsatım olursa bu kısmı ona göre düzelteceğim.

## Kaynaklar

- İlan: <https://twm.com.tr/tr/ilan/luna-1300-pro-firca-zimpara-makinesi>
- Üretici sayfası: <https://baromak.com.tr/urun-detay.html?id=luna-1300-pro>
