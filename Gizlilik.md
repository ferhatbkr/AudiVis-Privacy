# UDF+ Gizlilik Politikası

Bu gizlilik politikası, **UDF+** adlı Android uygulamasının kullanıcı verilerini, belgelerini ve cihaz kaynaklarını nasıl işlediğini, sakladığını ve koruduğunu açıklamaktadır.

## 1. Uygulamanın Temel İşlevleri ve Çevrimdışı Çalışma
UDF+, kullanıcıların cihazlarında bulunan çeşitli belge formatlarını görüntülemek ve dönüştürmek amacıyla tasarlanmış bir araçtır. Aşağıdaki temel işlemler **tamamen internet bağlantısı gerektirmeksizin, yerel olarak cihaz üzerinde (on-device)** gerçekleştirilir:
* UDF, PDF ve TIFF formatındaki belgelerin görüntülenmesi.
* DOC, DOCX ve RTF formatındaki belgelerin UDF formatına dönüştürülmesi.

## 2. Optik Karakter Tanıma (OCR) İşlemleri ve İnternet Kullanımı
Uygulama, taranmış belgelerdeki metinleri tanımak için iki farklı OCR yöntemi sunar:

* **Basit OCR (Çevrimdışı):** TIFF ve gerektiğinde PDF belgeleri için cihaz içi yerel kütüphaneler kullanılarak yapılır. Bu işlem sırasında hiçbir belge veya veri cihaz dışına aktarılmaz.
* **Gelişmiş OCR (Çevrimiçi):** Kullanıcının **kendi inisiyatifiyle** ilgili seçeneği aktif etmesi ve kendisine ait geçerli bir API anahtarı (API Key) sağlaması durumunda kullanılır. Bu özellik etkinleştirildiğinde, yalnızca metni tanınacak belgelerin görüntüleri işlenmek üzere Google Gemini API'sine iletilir. Bu veriler UDF+ geliştiricisine ait hiçbir sunucuda depolanmaz, kaydedilmez veya üçüncü şahıslarla paylaşılmaz. Veri aktarımı doğrudan kullanıcının cihazı ile Gemini servisleri arasında gerçekleşir.

## 3. Veri Saklama ve Önbellek (Cache) Yönetimi
Kullanıcı deneyimini iyileştirmek, cihaz kaynaklarını (batarya, işlemci) korumak ve aynı belge tekrar açıldığında yeniden işlem yapılmasını veya API kotası tüketilmesini önlemek amacıyla yerel bir önbellek mekanizması kullanılır.
* **Veri Tutma Kapasitesi:** Yalnızca son 100 belgeye ait Basit veya Gelişmiş OCR sonuçları cihazın kendi belleğinde yerel olarak saklanır.
* **Kullanıcı Kontrolü:** Kullanıcılar, uygulamanın ayarlar menüsü üzerinden diledikleri zaman bu önbelleği tamamen silebilir veya önbellek (cache) tutma özelliğini tamamen devre dışı bırakabilirler.

## 4. Toplanan Kişisel Veriler
UDF+; kullanıcıları tanımlayabilecek ad, soyad, e-posta adresi, konum bilgisi, cihaz tanımlayıcıları veya kullanım istatistikleri gibi **hiçbir kişisel veriyi toplamaz, işlemez veya saklamaz.** Uygulamanın eriştiği dosyalar, yalnızca kullanıcının açıkça seçtiği belgelerle sınırlıdır ve bu belgeler (Kullanıcının kendi sağladığı API anahtarıyla yaptığı Gelişmiş OCR istekleri haricinde) kapalı devre olarak sadece cihaz içinde kalır.

## 5. Üçüncü Taraf Kütüphaneler ve Veri Paylaşımı
Uygulama içerisinde belge görüntüleme, dönüştürme ve yerel OCR işlemleri için kullanılan üçüncü taraf kütüphaneler; hiçbir kullanıcı verisi toplamaz ve analitik veya reklam amacıyla veri paylaşımı yapmaz. Gelişmiş OCR için kullanılan Gemini API'nin veri işleme standartları ise Google'ın kendi gizlilik politikalarına ve kullanıcının API kullanımı şartlarına tabidir.

## 6. Kullanıcı Hakları
Uygulama tarafından geliştirici sunucularına iletilen hiçbir kişisel veya belgesel veri bulunmadığından, merkezi bir sistemden veri silme talebine gerek yoktur. Kullanıcılar, cihazlarındaki uygulama verilerini temizleyerek veya uygulamayı kaldırarak tüm verilerini ve ayarlarını anında yok edebilirler.

## 7. İletişim
Bu gizlilik politikası veya uygulamanın veri işleme yöntemleriyle ilgili her türlü sorunuz için aşağıdaki adres üzerinden iletişime geçebilirsiniz:

* **E-posta:** audivisplayer@gmail.com
