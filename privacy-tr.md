# Gizlilik Bildirimi - AudiVis Player

**Son Güncelleme:** 27 Aralık 2024

## Genel Bakış

AudiVis Player, gizliliğinize saygı duyar ve **hiçbir kişisel veri toplamaz, saklamaz veya üçüncü taraflarla paylaşmaz**.

## Veri Toplama

Bu uygulama:
- ❌ Kişisel bilgi toplamaz
- ❌ Kullanım istatistikleri göndermez
- ❌ Analitik servisleri kullanmaz
- ❌ Reklam göstermez
- ❌ Hesap oluşturma gerektirmez

## İzinler ve Kullanım Amaçları

### 📁 Depolama İzinleri
**İzinler:**
- `READ_EXTERNAL_STORAGE`
- `READ_MEDIA_VIDEO`
- `MANAGE_EXTERNAL_STORAGE`

**Amaç:** Cihazınızdaki video ve altyazı dosyalarını okumak için kullanılır.

**Veri Paylaşımı:** Hayır. Tüm dosyalar cihazınızda kalır.

### 🌐 İnternet Erişimi
**İzin:** `INTERNET`

**Amaç:** FTP ve SMB protokolleri üzerinden uzak sunuculardaki medya dosyalarına erişim için kullanılır.

**Veri Paylaşımı:** Hayır. Uygulama herhangi bir sunucuya veri göndermez.

**Not:** Analitik, reklam veya izleme servisleri kullanılmaz.

### 📶 Ağ Durumu
**İzinler:**
- `ACCESS_WIFI_STATE`
- `ACCESS_NETWORK_STATE`

**Amaç:** Ağ bağlantısının mevcut olup olmadığını kontrol etmek için kullanılır.

**Veri Paylaşımı:** Hayır.

### 🎵 Ön Plan Servisi
**İzinler:**
- `FOREGROUND_SERVICE`
- `FOREGROUND_SERVICE_MEDIA_PLAYBACK`
- `WAKE_LOCK`

**Amaç:** Arka planda video oynatmaya devam etmek ve bildirim göstermek için kullanılır.

**Veri Paylaşımı:** Hayır.

### 🔊 Metinden Sese (TTS)
**İzin:** `TTS_SERVICE` (query)

**Amaç:** Altyazıları sesli okumak için cihazınızdaki sistem TTS motorunu kullanır.

**Veri Paylaşımı:** TTS motoru tarafından işlenen veriler, kullandığınız TTS sağlayıcısının gizlilik politikasına tabidir (örn: Google TTS, Samsung TTS).

## Veri Güvenliği

### Yerel Depolama
- Tüm uygulama verileri cihazınızda yerel olarak saklanır
- Hiçbir veri bulut sunucularına yüklenmez

### Sunucu Kimlik Bilgileri
- FTP/SMB sunucu kimlik bilgileri Android'in `EncryptedSharedPreferences` API'si ile şifrelenmiş olarak saklanır
- Bu bilgiler yalnızca cihazınızda kalır ve asla paylaşılmaz

### Ağ Güvenliği
- Uygulama yalnızca sizin yapılandırdığınız FTP/SMB sunucularına bağlanır
- Hiçbir üçüncü taraf sunucuya bağlantı yapılmaz

## Üçüncü Taraf Hizmetler

AudiVis Player **hiçbir üçüncü taraf hizmeti kullanmaz**:
- ❌ Google Analytics yok
- ❌ Firebase yok
- ❌ Reklam ağları yok
- ❌ Çökme raporlama servisleri yok

**İstisna:** Cihazınızın sistem TTS motoru (kullanıcı tarafından seçilir).

## Çocukların Gizliliği

Bu uygulama 13 yaşın altındaki çocuklardan bilerek veri toplamaz. Uygulama herhangi bir yaş doğrulaması gerektirmez ve hiçbir kullanıcı verisini toplamaz.

## Değişiklikler

Bu gizlilik bildirimi zaman zaman güncellenebilir. Değişiklikler bu sayfada yayınlanacaktır.

## İletişim

Gizlilik ile ilgili sorularınız için:
- **GitHub:** https://github.com/ferhatbkr/AudiVis-Privacy/issues

## Açık Kaynak

AudiVis Player açık kaynak bir projedir:
- **Lisans:** Apache License 2.0
- **Kaynak Kod:** https://github.com/ferhatbkr/audivis-player

---

**Özet:** AudiVis Player tamamen çevrimdışı çalışan, gizliliğe saygılı bir video oynatıcıdır. Verileriniz yalnızca cihazınızda kalır.
