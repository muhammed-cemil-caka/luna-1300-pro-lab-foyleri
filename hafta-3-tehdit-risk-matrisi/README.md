# Lab 3 · Threat & Risk + Risk Matrix

**Çıktı:** Risk Register  
**Makine:** Baromak LUNA 1300 PRO fırça zımpara  
**Ad Soyad:** Muhammed Cemil Çaka  
**Tarih:** 3. Hafta

PDF hâli: [hafta-3-tehdit-risk-matrisi.pdf](../pdf/hafta-3-tehdit-risk-matrisi.pdf)

> **Kavram:** Senaryo beş parçadır: **kim → hangi kapı → ne yapar → zincir → FİZİKSEL sonuç**. Skor = L × S × E (her biri 1–3). **Kural:** S=3 ise skor düşük olsa bile senaryo öne alınır — insana zarar görünür kalır.

## Görev — üç senaryo kurun ve puanlayın

| # | Senaryo (kim → kapı → zincir → fiziksel sonuç) | L | S | E | Skor | Öncelik |
|---|---|:-:|:-:|:-:|:-:|:-:|
| 1 | **Dış saldırgan** (ele geçirilmiş ortak servis parolası) → üreticinin 7/24 açık uzaktan bağlantısı → HMI/PLC üzerinden fırça inverterinin duruş rampasını uzatır → kapak kilidi sabit süre bekleyip açılır → bakımcı çekmeceyi açtığında fırça hâlâ dönüyor, **el/kol fırçaya kaptırılır** | 2 | 3 | 3 | 18 (Kritik) | 1 |
| 2 | **Fidye yazılımı** (ofiste açılan e-posta eki) → ofis ile makine ağı ayrı değil → HMI kilitlenir, kayıtlı reçeteler kaybolur → operatörler baskı ayarını tahminen elle girer, fazla baskı verilir → ince parça sıkışıp **geri fırlar**, operatöre çarpar; aşırı sürtünmeden **toz tutuşabilir** | 2 | 2 | 2 | 8 (Orta) | 3 |
| 3 | **Zararlı yazılımlı servis laptopu / USB** → mühendislik yazılımı → Safety PLC'de kilit gecikmesi kısaltılır veya bir kapak girişi köprülenir → koruyucu açıkken makine çalışabilir → **dönen fırçaya erişim, ağır yaralanma** | 1 | 3 | 1 | 3 (Düşük) | 2 |

Skor aralıkları: Kritik 18–27 · Yüksek 9–17 · Orta 4–8 · Düşük 1–3 (L: olasılık, S: şiddet, E: maruziyet)

### 1. En yüksek öncelikli senaryonuz hangisi? Bir cümleyle: neden bu?

Birinci senaryo (uzaktan rampa değişikliği): bağlantı zaten var ve sürekli açık, sonucu kol kaybı ve bakımcı o çekmeceyi her vardiya açıyor.

### 2. S=3 olup skoru düşük kalan senaryonuz var mı? Nasıl görünür kılacaksınız?

Var, 3. senaryo. Skoru 3 (düşük) ama S=3 olduğu için öncelikte 2. sıraya aldım. Risk register'da bu satıra kırmızı "S=3" etiketi koyarım, her revizyonda ilk bakılan satır olur. Ayrıca safety programının checksum'ı devreye almada not edilsin ve periyodik bakım formunda "checksum aynı mı?" kontrolü olsun; bu kontrol yapılmadan satır kapanmasın.

> **Altın kural:** Zincir "veri çalındı" ile bitiyorsa emniyet bulgusu değildir — bir adım daha gidin: bu, hattaki insana ne yapar?

_Not: 2. senaryoyu ilk yazdığımda "reçeteler şifrelendi" diye bitiriyordum. Altın kurala göre bir adım daha ileri götürüp hattaki operatöre ne olacağını yazdım._

---

_Bu föyün çıktısı **Risk Register** → Evidence Pack **EP 04 Risk Assessment** başlığına oturur._
