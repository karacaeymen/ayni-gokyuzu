# ✦ Aynı Gökyüzü — Sevgiline Özel Aşk Sitesi Şablonu

Uzak mesafe ilişkisi olanlar (ya da sadece sevdiğine unutulmaz bir sürpriz yapmak isteyenler) için
hazırlanmış, **tek dosyalık, kurulum gerektirmeyen** romantik bir hediye sitesi.

Kod bilgisi gerekmez: tek bir dosyadaki metinleri değiştirir, fotoğraflarını klasöre atar,
siteyi ücretsiz yayınlarsın. 5 dakikada sevgiline özel bir link hazır.

---

## Özellikler

| | |
|---|---|
| 🔐 **Özel giriş ekranı** | Kullanıcı adı ve şifreyle açılan, girişte kalp/yıldız yağmuru yapan kapı |
| ⏳ **Geri sayım** | Buluşacağınız güne kalan gün, saat, dakika, saniye |
| 📖 **Hikayemiz** | İlişkinizin önemli anlarını gösteren zaman çizelgesi |
| 💬 **Bugünün Sözü** | Her gün değişen romantik bir cümle |
| 🎵 **Bugünün Şarkısı** | Her gün listeden seçilen bir şarkı + isteğe bağlı Spotify playlist'i |
| ❓ **Bugünün Sorusu** | İkiniz de aynı soruyu cevaplarsınız; cevaplar ancak ikiniz de yazınca açılır |
| 🙂 **Ruh hali takvimi** | Her gün nasıl hissettiğinizi seçin, son 90 gün renkli bir takvimde görünsün |
| 💝 **Sürpriz butonu** | "Seni neden sevdiğimi söyleyeyim" — her tıklamada başka bir sebep |
| 📸 **Anılarımız** | Polaroid görünümlü fotoğraf galerisi, tıklayınca büyür |
| 🃏 **Anı eşleştirme oyunu** | Kendi fotoğraflarınızla oynanan hafıza oyunu |
| 💍 **"Sonsuza kadar benimle olur musun?"** | "Hayır" butonu kaçar 😄 "Evet" deyince yazdırılabilir bir **Sonsuza Kadar Sertifikası** açılır |
| ✅ **Seninle yapmak istediğim şeyler** | İkinizin de ekleyip üstünü çizebildiği ortak dilek listesi |
| ✉️ **Not bırak** | Sevgilinin yazdığı notlar doğrudan e-postana gelir |
| 🌠 **Gizli yıldızlar** | Gökyüzünde saklı yıldızları bulunca özel bir sürpriz mektup açılır |
| 💫 **Kayan yıldızlar** | Ara sıra geçen kayan yıldıza tıklayınca küçük bir dilek çıkar |
| 🎉 **Kilometre taşı kutlamaları** | 100., 200., 365. gününüzde siteye girince otomatik kutlama |
| 🌌 **Yaşayan gökyüzü** | Saate göre renk değiştiren gökyüzü, telefonu eğince kayan yıldızlar |
| 🌗 **Açık / koyu tema** | Tek dokunuşla tema değişimi |
| 📱 **Mobil uyumlu** | Telefonda ana ekrana eklenince uygulama gibi açılır |
| 🔗 **QR kod ile paylaşım** | Sitenin linki ve QR kodu sayfanın sonunda |
| 🎶 **Arka plan müziği** | İsteğe bağlı, kendi şarkını ekleyebilirsin |

**Demo girişi:** kullanıcı adı `demo`, şifre `1234`

---

## Hızlı başlangıç

1. Bu depoyu indir (yeşil **Code** butonu > **Download ZIP**) ve zip'i aç.
2. `index.html` dosyasına çift tıkla, site tarayıcında açılır. Hepsi bu kadar, kurulum yok.
3. Kendine göre düzenle (aşağıda), sonra yayınla.

## Kişiselleştirme

`index.html` dosyasını Not Defteri veya VS Code ile aç ve
**`İÇERİĞİ BURADAN KOLAYCA DÜZENLEYEBİLİRSİN`** yazan bölümü bul. Sadece tırnak içindeki metinleri
değiştirmen yeterli:

| Ayar | Ne işe yarar |
|---|---|
| `NAME_1`, `NAME_2` | Senin ve sevgilinin adı; sitenin her yerinde kullanılır |
| `GATE_USER`, `GATE_PASS` | Giriş ekranının kullanıcı adı ve şifresi |
| `TARGET_DATE` | Geri sayımın hedef tarihi (buluşma günü) |
| `QUOTES` | Her gün gösterilecek sözler |
| `SONGS`, `PLAYLIST_ID` | Günün şarkısı listesi ve altta gösterilecek Spotify playlist'i |
| `DAILY_QUESTIONS` | "Bugünün Sorusu" soruları |
| `TIMELINE` | Hikayenizin tarihleri ve açıklamaları |
| `RELATIONSHIP_START_DATE`, `MILESTONE_DAYS` | Birlikteliğin başlangıcı ve kutlanacak gün sayıları |
| `REASONS` | "Seni neden seviyorum" sebepleri |
| `WISHES` | Kayan yıldız dilekleri |
| `SECRET_STARS`, `SECRET_REWARD_TITLE`, `SECRET_REWARD_TEXT` | Gizli yıldızların sözleri ve hepsi bulununca açılan mektup |
| `MEMORY_WIN_MESSAGES`, `MEMORY_PAIR_COUNT` | Anı oyunu kutlama mesajları ve kaç çiftle oynanacağı |
| `FOREVER_REVEAL_TEXT` | "Evet" denince çıkan mesaj |
| `MOODS` | Ruh hali seçenekleri ve renkleri |
| `SITE_URL` | QR kodda gösterilecek adres (boşsa sitenin o anki adresi) |
| `FIREBASE_CONFIG` | Ortak bölümler için (aşağıya bak) |
| `WEB3FORMS_ACCESS_KEY` | "Not Bırak" formu için (aşağıya bak) |

### Fotoğraflar

`images` klasöründeki `1.jpg` … `12.jpg` örnek görsellerini kendi fotoğraflarınla değiştir
(isimler aynı kalmalı). Daha fazla ya da daha az fotoğraf için `PHOTO_COUNT` değerini değiştir.
Anı eşleştirme oyunu da bu fotoğrafları kullanır.

### Arka plan müziği (isteğe bağlı)

`audio` adında bir klasör oluşturup içine `love-song.mp3` koyarsan sağ alttaki nota butonu çalışır.
Dosya yoksa buton kendiliğinden gizlenir.

### Ana ekran ikonu

`images/apple-touch-icon.png` dosyasını aynı isimle 180x180 boyutunda başka bir PNG ile
değiştirebilirsin.

---

## Ortak bölümler: Firebase kurulumu (isteğe bağlı, ücretsiz)

"Seninle Yapmak İstediğim Şeyler", "Bugün Nasılsın?" ve "Bugünün Sorusu" bölümleri Firebase
olmadan da çalışır, ama veriler **sadece o tarayıcıda** saklanır. İkinizin de aynı verileri
görmesi için:

1. [console.firebase.google.com](https://console.firebase.google.com) adresinde ücretsiz bir proje oluştur.
2. Sol menüden **Firestore Database > Create database** de.
3. **Rules** sekmesine şunu yapıştırıp **Publish** de:

   ```
   rules_version = '2';
   service cloud.firestore {
     match /databases/{database}/documents {
       match /{col}/{doc} {
         allow read, write: if col in ['wishlist', 'moods', 'dailyAnswers'];
       }
     }
   }
   ```

4. **Project settings > Your apps > Web (`</>`)** ile bir web uygulaması ekle. Sana verdiği
   `firebaseConfig` değerlerini `index.html` içindeki `FIREBASE_CONFIG` alanlarına kopyala.

Siteye ilk girişte "Sen kimsin?" diye bir kez sorulur; böylece ruh hali ve günün sorusunda
ikinizin cevapları ayrı görünür. Sayfanın en altındaki "kimsin? değiştir" ile değiştirilebilir.

## "Not Bırak" formu: Web3Forms kurulumu (ücretsiz)

1. [web3forms.com](https://web3forms.com) adresine e-posta adresini yaz, sana bir **Access Key** gelir.
2. Bu key'i `index.html` içindeki `WEB3FORMS_ACCESS_KEY` alanına yapıştır.

Artık sevgilinin bıraktığı notlar doğrudan e-postana düşer. Hesap veya kredi kartı gerekmez.

---

## Ücretsiz yayınlama (Netlify)

1. [app.netlify.com](https://app.netlify.com) adresinde ücretsiz hesap aç.
2. **Add new site > Deploy manually** de.
3. Bu klasörün tamamını tarayıcıdaki kutunun üzerine sürükle bırak.
4. Netlify sana `https://senin-siten.netlify.app` gibi bir adres verir, anında çalışır.

Güncelleme yapmak için klasörü tekrar **Deploys** sekmesine sürükle bırakman yeterli.

### Kendi domainini bağlamak (isteğe bağlı)

Netlify'da **Site configuration > Domain management > Add a domain** kısmından domainini ekle.
Netlify'ın verdiği nameserver adreslerini (ya da A / CNAME kayıtlarını) domaini aldığın firmanın
panelinde güncelle. Değişiklikler genelde birkaç saat, en geç 24-48 saat içinde aktif olur.

---

## Bilmen gerekenler

- **Giriş ekranı gerçek bir güvenlik değildir.** Kullanıcı adı ve şifre sayfanın kaynağında
  açıkça durur; hediye linkini meraklı gözlerden uzak tutmak için hafif bir kilittir. Siteye
  gizli kalması gereken bilgi koyma.
- Firebase `apiKey` değeri de sayfa kaynağında görünür; bu Firebase için normaldir. Yukarıdaki
  kurallar sadece sitenin kullandığı üç koleksiyona izin verir.
- Telefonu eğince kayan yıldızlar iPhone'da ilk dokunuşta izin ister ve sadece `https`
  adreslerinde (yayınlandıktan sonra) çalışır.
- Sertifikadaki **Yazdır / PDF Kaydet** butonu, telefonun yazdırma ekranından PDF olarak
  kaydetmeye de izin verir.

Her şey tek bir `index.html` dosyasında: build, sunucu ya da paket kurulumu yok.
