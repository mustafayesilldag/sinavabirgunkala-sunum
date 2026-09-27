# Sunum maddeleri nasıl düzenlenir

Sayfadaki geliştirme maddeleri `maddeler.js` dosyasından okunur. Özet tablosu, madde kartları, numaralar, "X yeni özellik" sayısı ve yol haritası bu dosyaya göre kendiliğinden oluşur.

## Görsel düzenleyici (önerilen)

1. Sayfayı adresin sonuna `?duzenle` ekleyerek açın.
   Örnek: `https://kullaniciadi.github.io/repo-adi/?duzenle`
2. Her maddenin sağ üstünde düğmeler vardır:
   - **↑ ↓**: maddeyi yukarı ya da aşağı taşır
   - **Düzenle**: sağda düzenleme panelini açar
   - **Gizle**: maddeyi silmeden müşteriden saklar
   - **Sil**: maddeyi tamamen kaldırır
3. Alttaki çubuktan **+ Yeni madde** ile madde ekleyin.
4. Düzenleme panelinde şunları yapabilirsiniz:
   - Başlık, açıklama, kazanç, özellikler ve bilgi kutularını yazmak
   - Fotoğraf eklemek (sürükleyip bırakın ya da tıklayıp seçin)
   - Çerçeve seçmek: Kart, Tarayıcı penceresi, Işıklı kenar ya da Çerçevesiz
   - Yerleşim seçmek: Otomatik, Görsel sağda, Görsel solda, Görsel üstte, Görsel altta ya da Sadece yazı
   - Yol haritasında hangi aşamada görüneceğini seçmek
5. **Müşteri görünümü** düğmesi, sayfanın müşteriye nasıl görüneceğini gösterir.
6. İşiniz bitince **maddeler.js indir** düğmesine basın.
7. GitHub'da repoda **Add file → Upload files** ile indirdiğiniz `maddeler.js`'i yükleyin; eskisinin yerine geçer. **Commit changes** deyin. Birkaç dakika içinde yayındaki sayfa güncellenir.

Değişiklikler, dosyayı indirene kadar yalnızca kendi tarayıcınızda taslak olarak durur. Sayfayı kapatsanız da taslak kaybolmaz. **Taslağı sil**, yayındaki hale geri döndürür.

Fotoğraflar küçültülüp `maddeler.js`'in içine gömülür, ayrıca yüklemeniz gerekmez. İsterseniz fotoğrafı `gorseller/` klasörüne yükleyip panelde "dosya yolu" alanına `gorseller/dosya-adi.jpg` yazabilirsiniz.

## GitHub üzerinden doğrudan düzenleme

Küçük yazı düzeltmeleri için `maddeler.js` dosyasını GitHub'da kalem simgesiyle açıp düzenleyebilirsiniz. Tırnak işaretlerine ve satır sonlarındaki virgüllere dokunmayın. Emin olamadığınız değişiklikler için görsel düzenleyiciyi kullanın.

| Alan | Ne işe yarar |
|---|---|
| `baslik` | Madde kartındaki başlık |
| `kisa_baslik` | Özet tablosundaki ad (boşsa başlık kullanılır) |
| `ozet` | Özet tablosundaki tek cümle |
| `aciklama` | Kartın açıklama paragrafı |
| `kazanc` | "Siteye kazancı" cümlesi |
| `ozellikler` | Tik işaretli maddeler |
| `kutular` | Küçük bilgi kutuları (başlık + metin) |
| `kimler` | Kimler için etiketleri |
| `asama` | Yol haritası aşaması (1–4) |
| `gorsel.tur` | `hazir` (sayfaya özel çizim), `resim` ya da `yok` |
| `yerlesim` | `otomatik`, `sag`, `sol`, `ust`, `alt`, `yok` |
| `cerceve` | `kart`, `tarayici`, `parlak`, `yok` |
| `gizli` | `true` ise madde müşteriye görünmez |
