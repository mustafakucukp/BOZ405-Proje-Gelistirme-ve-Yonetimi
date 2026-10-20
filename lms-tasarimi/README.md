# BOZ405 Proje Geliştirme ve Yönetimi

## LMS Kaynak Yönetimi için Hızlı Tasarım Sprinti

* **Ad Soyad:** Mustafa KÜÇÜKPARLAK
* **Öğrenci No:** 23040342
* **Tarih:** 20 Ekim 2026
* **Süreç:** Mühendislik Tasarım Süreci'nin 5 aşaması (Empati → Tanımla → Fikir Üret → Prototiple → Test Et) 120 dakikalık bir sprintte uygulanmıştır.
* **Senaryo:** Üniversitenin LMS'indeki (Moodle, Canvas vb.) "Kaynaklar/Dosyalar" bölümü çok uzundur. PDF, video ve linkler kronolojik veya alfabetik tek bir listede sıralanır; öğrenciler kaynak bulmakta zorlanır, motivasyonları düşer ve zaman kaybederler.

---

### 1. Empati Haritası

**Persona:** LMS'te (Moodle/Canvas) ders kaynaklarına sık başvuran bir üniversite öğrencisi. Harita, kendi öğrencilik deneyimlerime dayanmaktadır.

<img width="1024" height="768" alt="Empati_haritası" src="https://github.com/user-attachments/assets/b174bd34-b770-485e-871e-25c2cbfac8aa" />




---

### 2. Problem Cümlesi ve HMW Sorusu

* **Problem Cümlesi:** Üniversite öğrencisi, sınav kapsamı ve ders kazanımlarıyla doğrudan ilişkilendirilmiş önizlemeli ve filtreli bir kaynak merkezine ihtiyaç duyuyor; çünkü kronolojik/alfabetik uzun dosya listelerinde aradığı bilginin hangi dosyanın içinde olduğunu kestiremiyor ve dosyaları tek tek indirip kontrol etme eforu asıl çalışma motivasyonunu tüketiyor.
* **HMW (Nasıl Yapabiliriz?) Sorusu:** Öğrencilerin dosya indirme ve arama bariyerini ortadan kaldırıp, ders kaynaklarını sınav hedefleriyle eşleşen ve anında önizlenebilen dinamik bir çalışma alanına nasıl dönüştürebiliriz?

---

### 3. Beyin Fırtınası ve Seçim

| # | Fikir Başlığı ve Açıklaması |
|---|---|
| 1 | **Kazanım & Modül Odaklı Kart Görünümü** (Haftalık liste yerine ünite/hedef odaklı bloklar) |
| 2 | **Sayfa Değiştirmeden Anlık Modal Önizleme** (PDF'i indirmeden içini açıp tarama) |
| 3 | **Kişisel Çalışma Masası** (Pinleme & Not Ekleme) |
| 4 | **Dinamik Sınav Kapsamı Filtresi** (#Vize, #Final, #Zorunlu, #Özet) |
| 5 | **Tahmini Okuma Süresi ve Sayfa Sayısı Rozetleri** |
| 6 | **Toplu İndirme (.ZIP) Sepeti** (Seçilenleri tek pakette alma) |
| 7 | **LMS İçi Arama ve Doğal Dil Sohbet Asistanı** |
| 8 | **Kitle Kaynaklı Yıldızlama / Sınav Favorileri** |
| 9 | **Konu Ağacı / Zihin Haritası Görünümü** |
| 10 | **Haftalık İlerleme ve Tamamlanma Çubuğu** |

#### Seçilen Çözüm
Fikir 1+2+3+5 birleşimi: **"Sınav Modlu Konu Haritası"**. Kaynaklar haftalara göre kartlarda gruplanır, türe göre filtrelenir; "Sınav Modu" açılınca öğrencilerin faydalı bulduğu ve sınavla ilişkili kaynaklar öne çıkar. Kullanıcı kaynakları kaydedip not ekleyebilir ve ilerlemesini görür.

#### Seçim Gerekçesi
* **HMW'ye doğrudan cevap veriyor:** Problem "neyin önemli olduğunu bilememek"; Sınav Modu tam bu belirsizliği gideriyor.
* **Düşük sadakatle test edilebilir:** 3 ekranla bütün akış (gez, filtrele, kişiselleştir) 40 dakikada çizilebiliyor.
* **Mevcut LMS'e uygulanabilir:** Sohbet botu veya ses asistanı gibi fikirler ek altyapı gerektirirken bu çözüm etiket, filtre ve oylama ile kurulabilir. Uçuk fikirler (6, 8, 9, 10) bu sprintte elendi ancak ileride eklenebilecek tohumlar olarak not edildi.

---

### 4. Prototip Ekran Tasarımları

#### 1. Sınav Modlu Konu Haritası ve Modüler Kaynaklar (Ana Sayfa)
<img width="939" height="416" alt="image" src="https://github.com/user-attachments/assets/821f8b09-9a6a-4675-8364-1af96f5c203c" />


#### 2. Dosya İçi Hızlı Önizleme ve İterasyon Not Modalı
<img width="939" height="505" alt="image" src="https://github.com/user-attachments/assets/ce71c9b9-7732-47e3-ba55-65f1ef64604d" />


#### 3. Kişisel "Çalışma Masam" ve Sınav Hazırlık Panosu
<img width="939" height="417" alt="image" src="https://github.com/user-attachments/assets/f8a2fabd-a1be-48d7-9533-40cda31bddbd" />


---

### 5. Test Sonuçları

* **Test Edilen Kişi:** Ceylan Ulusoy
* **Verilen Görev:** "Önümüzdeki hafta yapılacak vize sınavı için 'Öğrenme Tasarımı' konusuna ait özet slaytı bul, bilgisayarına indirmeden içeriğine göz at ve sınav panona iğnele."

#### En Önemli 2 Geri Bildirim:
1. **İndirmeden İnceleme Kolaylığı:** Önizleme penceresinin sayfa değiştirmeden doğrudan açılmasının muazzam bir hız kazandırdığını; daha önce "acaba aradığım bu mu" diye 5 farklı PDF indirip silmek zorunda kaldığını, bu sistemde 10 saniye içinde doğru kaynağı onaylayıp masasına alabildiğini belirtti.
2. **Kişisel Not Alanının Konumu:** İlk testte "Masama İğnele" butonu ile "Not Ekle" alanının birbirinden kopuk olduğunu, iğneledikten sonra karta geri dönüp not yazmaya çalışırken kafasının karıştığını söyledi.

* **Yapılan İterasyon:** Kullanıcı geri bildirimi doğrultusunda, önizleme modalı içine doğrudan **"İğnele ve Hatırlatma Notu Bırak"** bileşeni entegre edildi. Öğrenci belgeyi incelerken sağ tarafa doğrudan "Sayfa 14'teki tablo sınavda çıkacak" yazıp kaydettiğinde, belge notuyla birlikte otomatik olarak Çalışma Masası'na aktarılacak şekilde arayüz sadeleştirildi.

---

### 6. Bireysel Öğrenim Yansıması

* **En Önemli Öğrenimim:** Kullanıcı testinde gördüğüm en kritik içgörü; öğrencilerin yaşadığı stresin kaynak yetersizliğinden değil, aksine "kaynak enflasyonu ve belirsizlik"ten kaynaklandığı oldu. Öğrenci sisteme girdiğinde bir kütüphane arşiviyle değil, hedefine rehberlik eden, neyin öncelikli olduğunu hissettiren filtreli bir zihinsel modelle karşılaşmak istiyor.
* **Sürece Dair Yansıma:** Mühendislik Tasarım Süreci'ni 120 dakikalık yoğun bir sprintte deneyimlemek, bir problemi çözerken ilk akla gelen fikre (örneğin hemen karmaşık bir yapay zekâ botu yapmaya kalkışmak gibi) körü körüne bağlanmamayı öğretti. Empati ve Tanımla aşamasına ayrılan 25 dakikalık odaklanma, problemin kökündeki "dosya indirme sürtünmesi"ni görmemi sağladı. Düşük sadakatli bir prototip üzerinden alınan tek bir akran geri bildirimi bile, haftalarca masa başında tahmin yürüterek ulaşılamayacak bir tasarım berraklığı sundu.
