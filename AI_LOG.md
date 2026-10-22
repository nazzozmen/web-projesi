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

💬 Oturum 2: Proje Dokümantasyonu ve Sunum Metinleri

🔹 2. Soru (Kullanıcı Girdisi)

"Bana bu projenin konusu, amacı, hedefleri, kapsamı ve temel özelliklerini içeren, sunum dosyama ekleyebileceğim kurumsal ve akademik bir tanım metni hazırlar mısın?"

🤖 Yapay Zeka Cevabı (Özet)

Proje akademik standartlara uygun olarak Proje Konusu, Proje Amacı, Projenin Hedefleri, Kapsam İçi / Kapsam Dışı Analizi ve Hoca / Öğrenci / Teknik Modül Özellikleri başlıkları altında detaylı bir şekilde raporlandı.

🎯 Projede Kullanım Alanı (Nasıl Kullanıldı?)

Sunum Dosyasının Hazırlanması: Cevaptaki maddeler doğrudan sunum slaytlarının (Giriş, Amaç, Kapsam ve Özellikler) ana metni olarak kullanıldı.

Proje Sınırlarının Belirlenmesi: Kapsam içi ve kapsam dışı maddeleri sayesinde projenin ilk etapta e-posta odağında tutulması, ücretli SMS sistemlerinin ise 2. faza bırakılması kararlaştırıldı.

💬 Oturum 3: Teknik Detaylar ve Performans Optimizasyonu

🔹 3. Soru (Kullanıcı Girdisi)

"Bu sistemde hoca tek tıkla 200 öğrenciye ders iptal e-postası attığında sistemin kilitlenmemesi ve maillerin spama düşmemesi için veritabanı ve arka yüz (backend) tarafında nasıl bir yapı kurmalıyım?"

🤖 Yapay Zeka Cevabı (Özet)

Toplu mail gönderimlerinde ana sunucunun kilitlenmemesi için Asenkron Kuyruk (Task Queue / Celery / Background Tasks) yapısının kullanılması, e-postaların spama düşmemesi için özel HTML şablonları ve SMTP/API servislerinin (Resend / Mailgun vb.) tercih edilmesi gerektiği belirtildi. Ayrıca kullanıcılar, dersler ve duyurular arasındaki ilişkileri gösteren temel bir veritabanı ilişki modeli önerildi.

🎯 Projede Kullanım Alanı (Nasıl Kullanıldı?)

Veritabanı Tasarımı (DB Schema): Veritabanı tabloları (Users, Courses, Announcements, Logs) oluşturulurken bu yanıttaki ilişkisel yapı referans alındı.

Sistem Performans Planlaması: Sunumun "Performans ve Güvenlik" bölümüne kuyruk mimarisinin avantajları eklendi.
