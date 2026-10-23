bu dosyaya web projesi dersi boyunca hafta hafta yapay zekaya yazdığımız promtları 
ve bize verdiği cevapları ve bu cevaplardan nasıl yararlanacağımızı not edeceğiz.
16 Ekim görevi


ai a sorduğum soru:

🔹 1. Soru
"Üniversitede hocaların öğrencilere kolay bir şekilde ulaşacağı, ders iptali ya da duyuru olunca siteye kayıt olan öğrencilere hızlıca haber veren bir web sitesi fikrim var. Böyle bir sistem nasıl çalışmalı ve temel mimarisi nasıl olmalı?"

🤖 Yapay Zeka Cevabı (Özet)

Sistemin genel işleyişi Rol Yönetimi (Hoca/Öğrenci) ve Duyuru Otomasyonu olarak ikiye ayrıldı. Backend tarafında asenkron e-posta kuyruk yapısı (Queue) ve SMTP entegrasyonu kullanılması gerektiği, frontend tarafında ise ders bazlı filtreleme ve acil durum renk kodlaması (örn: Ders iptali için kırmızı vurgu) yapılması gerektiği önerildi. Ayrıca sisteme ait temel bir mimari akış şeması sunuldu.

🎯 Projede Kullanım Alanı (Nasıl Kullanıldı?)

Proje Fikrinin Olgunlaştırılması: Projenin sadece basit bir web sitesi değil, arka planda e-posta motoru ve kuyruk sistemi çalışan bir iletişim otomasyonu olarak kurgulanması sağlandı.

Teknik Mimari Tasarımı: Sunumun teknik altyapı slaytında yer alan istemci-sunucu-mail servisi akış şeması bu yanıt doğrultusunda çizildi.


🎯 Projede Kullanım Alanı (Nasıl Kullanıldı?)

Veritabanı Tasarımı (DB Schema): Veritabanı tabloları (Users, Courses, Announcements, Logs) oluşturulurken bu yanıttaki ilişkisel yapı referans alındı.

Sistem Performans Planlaması: Sunumun "Performans ve Güvenlik" bölümüne kuyruk mimarisinin avantajları eklendi.
