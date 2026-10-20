# BOZ405 Proje Geliştirme ve Yönetimi
## LMS Kaynak Yönetimi için Hızlı Tasarım Sprinti

- **Ad Soyad:** CEYLAN ULUSOY
- **Öğrenci No:** 23040192
- **Tarih:** 20 Ekim 2026
- **Süreç:** Mühendislik Tasarım Süreci'nin 5 aşaması (Empati → Tanımla → Fikir Üret → Prototiple → Test Et) 120 dakikalık bir sprintte uygulanmıştır.
- **Senaryo:** Üniversitenin LMS'indeki (Moodle, Canvas vb.) "Kaynaklar/Dosyalar" bölümü çok uzundur. PDF, video ve linkler kronolojik veya alfabetik tek bir listede sıralanır; öğrenciler kaynak bulmakta zorlanır, motivasyonları düşer ve zaman kaybederler.

---

### 1. Empati Haritası (Persona: Üniversite öğrencisi)
![Empati Haritası](./empati-haritasi.png)

| Ne görüyor? | Ne duyuyor? |
| :--- | :--- |
| Kaynaklar bölümünde onlarca dosyanın uzun, düz bir listede sıralandığını; birbirine benzeyen dosya adlarını (Hafta3_son, Hafta3_son_v2); arkadaşlarının gruplarda "hocanın slaytı nerede?" diye sorduğunu. | Arkadaşları: *"Ben de bulamadım, grupta var mı?"*<br>Hoca: *"Tüm kaynaklar sisteme yüklü."*<br>Üst sınıflar: *"Dosyaları kendin indirip klasörle."* |

| Ne düşünüyor ve hissediyor? | Ne söylüyor ve yapıyor? |
| :--- | :--- |
| *"Bu dosyayı nerede görmüştüm?"* Bunalmış, sinirli; sınav öncesi *"bir şeyi kaçırıyor muyum?"* kaygısı. | Dosyaları tek tek açıyor, arkadaşlarından dosya istiyor, kendi bilgisayarında klasörlüyor, çalışmayı erteliyor. |

* **Acısı:** Doğru kaynağı bulmak için gereğinden fazla zaman harcıyor, hangi kaynağın önemli olduğunu bilmiyor, çalışma motivasyonu başlamadan düşüyor.
* **Kazancı:** Kaynağa birkaç saniyede ulaşmak, o hafta neyi çalışacağını net görmek, zamanını arayarak değil çalışarak geçirmek.

---

### 2. Problem Cümlesi ve HMW Sorusu

* **Problem Cümlesi:** Üniversite öğrencisi Elif, ders kaynaklarına hızlıca ulaşmaya ihtiyaç duyuyor; çünkü kaynaklar kronolojik veya alfabetik uzun listelerde sıralandığı için aradığını bulmakla geçen zaman, asıl çalışma zamanını ve motivasyonunu tüketiyor.
* **HMW (Nasıl Yapabiliriz?):** Öğrencilerin, ihtiyaç duydukları ders kaynağına birkaç saniye içinde ulaşıp o hafta neyi çalışmaları gerektiğini net görmelerini nasıl sağlayabiliriz?

---

### 3. Beyin Fırtınası ve Seçim

| # | Fikir | # | Fikir |
| :-: | :--- | :-: | :--- |
| **1** | Haftalık görünüm (kaynaklar hafta kartlarında) | **6** | Önem sırası rozeti (Mutlaka bak / Ek kaynak) |
| **2** | Akıllı arama çubuğu (konu, hafta, tür filtresi) | **7** | Sohbet botu ile kaynak yönlendirme |
| **3** | "Bu hafta çalış" paneli | **8** | Oyunlaştırma (ilerleme çubuğu, rozet) |
| **4** | Renkli etiket sistemi (Slayt, video, ödev) | **9** | Konu zihin haritası görünümü |
| **5** | Öğrenci favorileri / yıldız | **10** | Haftalık özet e-postası |

* **Seçilen Çözüm:** **Haftalık Kaynak Kartları (Fikir 1 + 2 + 3 + 4)**  
  Kaynaklar haftalara bölünür, ana sayfada "Bu hafta çalış" paneli yer alır, her dosya renkli bir tür etiketi taşır ve arama/filtre bileşenleriyle taranabilir.
* **Seçim Gerekçesi:** Seçim ölçütlerim problemin kök nedenini ne kadar çözdüğü ve 120 dakikalık sprintte prototiplenebilirliğiydi. Empati haritasındaki en büyük acı "uzun düz liste" olduğu için bu çözüm doğrudan hiyerarşik yapı kurarak onu hedefliyor. Sohbet botu ve e-posta gibi fikirler 120 dakikada prototiplenip test edilemeyecek kadar karmaşıktı.

---

### 4. Prototip Ekran Görüntüleri

#### Ekran 1: Ana sayfa ("Bu hafta çalış" paneli)
![Ekran 1 - Ana Sayfa](./assets/prototip-ekran-1.png)

#### Ekran 2: Tüm haftalar ve filtreler
![Ekran 2 - Tum Haftalar](./assets/prototip-ekran-2.png)

#### Ekran 3: Arama sonuçları
![Ekran 3 - Arama Sonuclari](./assets/prototip-ekran-3.png)

---

### 5. Test Sonuçları

* **Test Eden Kişi:** Mert (3. Sınıf Mühendislik Fakültesi Öğrencisi)
* **Görev:** *"Bu haftanın empati haritası sunumunu bul."*
* **En Önemli 2 Geri Bildirim:**
  1. Ana sayfadaki "Bu Hafta Çalış" paneli sayesinde arama bile yapmadan tek bakışta ilgili haftanın slaytına 3 saniye içinde ulaştı ve renkli etiketlerin dosya türünü ayırt etmede çok hız kazandırdığını belirtti.
  2. "Tüm Haftalar" ekranında önceki haftaların kartlarına bakarken, vize öncesi hangi kaynakları tamamlayıp hangilerini henüz açmadığını görebilmek için kartların üzerinde küçük bir tamamlama/okundu göstergesi aradığını ifade etti.
* **Yaptığım İterasyon:** 
  Hafta kartlarının alt kısmına ince bir yeşil "tamamlama/ilerleme çizgisi" eklendi; ayrıca arama sonuçları ekranında aranan kelimenin ("empati") hangi hafta kartından geldiği daha vurgulu ve belirgin rozetlerle gösterildi.

---

### 6. Bireysel Öğrenim Yansıması

* **En Önemli Öğrenimim:**
  Test aşamasında fark ettiğim en şaşırtıcı içgörü; öğrencilerin temel sorununun kaynağın sistemde var olup olmaması değil, **"bilişsel yük"** ve **"zaman belirsizliği"** olduğuydu. Kullanıcı sadece bir dosya listesi değil, o hafta kendisinden tam olarak ne beklendiğini özetleyen sade bir rehber arayüz istiyor.
* **Sürece Dair Yansıma:**
  Mühendislik Tasarım Süreci'nin beş aşamasını uygularken, doğrudan çözüm üretmeye atlamak yerine empati ve tanımlama aşamasında kök probleme odaklanmanın tasarım kararlarını ne kadar kolaylaştırdığını deneyimledim[cite: 1, 2, 4, 8, 9]. 120 dakikalık kısıtlı sürede fikirleri filtrelerken uygulanabilirlik kriterinin önemini gördüm; hızlı bir prototip üzerinden kullanıcı testi yapmanın ise varsayımlarla tasarım yapmaktan çok daha güvenilir sonuçlar verdiğini fark ettim[cite: 2, 8, 9].
