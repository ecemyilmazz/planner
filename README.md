# Planner

Yöneticiler için gün planlama aracı. Tek HTML dosyası, bağımlılık yok, sunucu yok.

**[Demoyu aç →](https://KULLANICI-ADIN.github.io/planner/)**

## Çözdüğü problem

Takvim uygulamaları her şeyi saat ızgarasına tıkıştırır. Oysa bir yöneticinin gününde iki farklı şey vardır:

- **Zaman kaplayan işler** — toplantılar, çalışma dilimleri, bireysel zaman. Bunların başlangıcı ve bitişi vardır.
- **Zaman kaplamayan işler** — son tarihi olan takipler. Bunlar günün belirli bir saatinde değildir, sadece o gün hatırlanması gerekir.

İkisini aynı ızgaraya koyunca takvim okunmaz hale gelir. Bu araç ayrımı **renkle değil konumla** yapar: hatırlatmalar sol rayda, ızgaranın tamamen dışında durur.

## Özellikler

- Gün görünümü — sol rayda hatırlatmalar ve atanmamış işler, sağda 15 dakikalık zaman ızgarası, canlı "şu an" çizgisi
- Hafta görünümü — 7 gün, üstte ayrı son tarih şeridi
- Kayıt tablosu — tür, departman, sorumlu ve metin araması
- Sürükle-bırak ile planlama; atanmamış havuzdan takvime, takvim içinde saat değiştirme
- `.ics` dışa aktarım — haftanın kayıtları Google Takvim / Outlook'a aktarılır, hatırlatma alarmlarıyla
- JSON yedek alma ve geri yükleme; 7 gün yedek alınmazsa uyarı
- Ayarlanabilir gün aralığı, 15/30 dakika dilim, isteğe bağlı alanlar

## Gizlilik

Sunucu yok, hesap yok, analitik yok. Girilen tüm veri kullanıcının kendi tarayıcısında (`localStorage`) kalır ve hiçbir yere gönderilmez. Aynı adresi açan iki kişi birbirinin verisini göremez.

Depodaki örnek kayıtlar tamamen kurgudur.

## Teknik

Bağımlılık yok, derleme adımı yok. Tek dosya: HTML + CSS + vanilla JS. Yazı tipleri Google Fonts üzerinden gelir, erişilemezse sistem yazı tiplerine düşer.

Yerelde çalıştırmak için `index.html` dosyasını tarayıcıda açmak yeterlidir.

## Lisans

MIT
