---
title: MeterLink Gizlilik Politikası
---
# MeterLink Gizlilik Politikası

**Son güncelleme:** 13 Eylül 2026

**Geliştirici:** Onur İmeci

**Gizlilik iletişimi:** onurimeci.dev@gmail.com

## 1. Kapsam ve amaç

MeterLink, uyumlu IEC 62056-21 elektrik sayaçlarını Bluetooth Classic veya USB Serial optik problarla okumaya yönelik bir saha uygulamasıdır. Bu politika, uygulamanın cihaz üzerindeki veri işleme davranışını açıklar.

## 2. Cihazda işlenen ve saklanan veriler

Uygulama kullanım sırasında şu operasyonel verileri cihazda işleyebilir ve saklayabilir:

- sayaç seri numarası, tesisat bilgisi ve IEC kimlik bilgileri;
- OBIS ölçüm değerleri ve yük profili değerleri;
- okuma zamanı, sonucu, kullanılan okuma modu ve cihaz ilişkisi;
- kayıtlı optik prob adı/türü, Bluetooth MAC adresi veya USB VID/PID/seri bilgisi;
- kullanıcının verdiği cihaz adları ve uygulama ayarları;
- tercihlere bağlı olarak özgün RAW sayaç iletişimi ve TX/RX tanılama kayıtları;
- kullanıcının açık talebiyle oluşturulan CSV, XLSX, RAW veya günlük dışa aktarımları.

Bu veriler Room veritabanında ve uygulamanın Android tarafından korunan özel dosya alanında yerel olarak tutulur. Büyük RAW ve günlük kanıtları veritabanı BLOB'u olarak saklanmaz.

## 3. Otomatik aktarım ve üçüncü taraflar

Mevcut uygulama sürümü ağ iletişimi kullanmaz ve INTERNET izni istemez. Kod ve bağımlılık denetimine göre analitik, reklam, crash-reporting veya bulut yükleme SDK'sı bulunmaz. Uygulama sayaç ya da cihaz verilerini geliştiriciye veya üçüncü taraflara otomatik olarak göndermez.

Kullanıcı **Paylaş** veya **Farklı Kaydet** işlemini açıkça başlatırsa seçilen veriler Android paylaşım/SAF arayüzü üzerinden kullanıcının seçtiği uygulamaya veya konuma aktarılır. Hedef hizmetin veri işleme koşulları kendi gizlilik politikasına tabidir.

## 4. Bluetooth, konum ve USB erişimi

- Bluetooth izinleri kayıtlı Bluetooth Classic probla bağlantı ve cihaz keşfi için kullanılır.
- Android 12 ve sonrasında tarama ve bağlantı izinleri ayrı istenir. Uygulama Bluetooth taramasını fiziksel konum çıkarmak için kullanmaz.
- Android 11 ve öncesinde Fine Location izni yalnız Bluetooth keşfinin platform gereksinimi nedeniyle istenir; konum verisi uygulama tarafından kaydedilmez.
- USB erişimi, kullanıcının bağladığı USB Serial prob için Android'in cihaz-bazlı izin akışıyla alınır.

## 5. Saklama ve silme

RAW ve tanılama dosyaları kullanıcı tarafından seçilen 7, 30, 90 gün veya süresiz saklama politikasına göre temizlenebilir. Yapılandırılmış okuma geçmişi, kullanıcı ilgili okuma/yük profili detayından silene kadar kalır. Bir optik cihaz kaydını silmek geçmiş okumaları otomatik olarak silmez.

Uygulama kaldırıldığında uygulama içindeki yerel veriler Android tarafından silinir ve Android yedeklemesi kapalıdır. Kullanıcının daha önce başka bir konuma aktardığı dosyalar uygulamanın kontrolü dışındadır ve hedef konumdan ayrıca silinmelidir.

## 6. Güvenlik

Operasyonel veriler varsayılan olarak uygulamaya özel depolamada tutulur. Dışa aktarım için yalnız `cache/exports/` alanındaki geçici dosyalar, süreli okuma izni olan `content://` URI'leriyle paylaşılır. Uygulama cleartext ağ trafiğine izin vermez. Bununla birlikte hiçbir elektronik saklama yöntemi mutlak güvenlik garantisi vermez; cihaz ekran kilidinin ve fiziksel erişimin korunması kullanıcı sorumluluğundadır.

## 7. Çocuklar

Uygulama profesyonel/operasyonel bir araçtır ve çocuklara yönelik olarak tasarlanmamıştır.

## 8. Politika değişiklikleri ve iletişim

Bu politika uygulama davranışı veya yasal gereksinimler değiştiğinde güncellenebilir. Güncel tarih ve metin uygulama içinde ve Google Play listelemesindeki herkese açık politika sayfasında yayımlanır. Sorular ve veri talepleri için onurimeci.dev@gmail.com adresine başvurulabilir.[](./)
