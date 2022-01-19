---
layout: default
title: Sistem Sıfırlama
description: "Mazaka Yazilim Eticaret Sistem Sifirlama Dokumantasyonu."
nav_order: 2
has_children: true
parent: Ayarlar
permalink: /docs/ayarlar/sistem-sifirlama
---

# Sistem Sıfırlama Kullanım Dökümantasyonu
Merhabalar bu dökümantasyonda panel üzerinden bir sistem nasıl sıfırlanır onu öğreneceğiz.

# Sistem Sıfırlama

İlk olarak panel üzerinde bulunan sol menüden **Sistem** > **Ayarlar** seçeneklerine ulaşıyoruz. Daha sonra önümüze çıkan **Ayarlar** sayfasının sağ üst tarafında kırmızı renkte bulunan **Sistem Sıfırlama** butonuna tıklıyoruz ve karşımızda bir popup beliriyor. 

Açılan popup içerisinde 6 adet seçenek ile karşılaşıyoruz. Bu seçenekleri üzerine gelip tıklama işlemi gerçekleştirdiğimizde yeşil renk olan seçenekler bizim seçtiğimiz seçenekler olmaktadır.

**1-) Kullanıcı Sıfırlama**
- Sistem içerisinde bulunan Admin yetkisi haricindeki  ve herhangi bir  yetkiye sahip kullanıcılar hariç bütün kullanıcılar silinir.
- Base role olmayan bütün roller silinir.
 
**2-) Tema Sıfırlama**
- İçerik yönetimi kullanılarak özelleştirilen bütün sayfalar silinir. 

**3-) Satış ve Ödeme Sıfırlama**
- Sistem üzerinde yapılmış olan bütün satışlar ve ödemeler silinir.
- Sistemde oluşturulmuş olan bütün sepetler silinir.
- Sistem oluşturulmuş olan bütün kampanyalar silinir.
- Sistemde oluşturulmuş olan bütün danışma ve randevu kayıtları silinir.

**4-) Ürün Sıfırlama**
- Sistem içerisinde bulunan bütün ürünleri siler ve ürüne bağlı sepet, satış, yorum ve indirimleri temizler.
- Sistem içerisindeki bütün envanter kayıtlarını, blog sayfalarını ve entegrasyonları temizler. 

**5-) Ayar Sıfırlama**
-	Sisteme ait bütün ayarlar ve şirket bilgileri silinir.
-	Sisteme kayıtlı olan ve bir role sahip bankalar silinir role sahip olmayan bankaların ise BusinessNo, BusinessPass , BusinessId ,BusinessKey , IBAN , IBAN Description ve BusinessUser alanları temizlenip pasif hale çekilir.
-	Aktif banka olarak Havale / EFT ve Varsayılan seçilir.

**6-) Medya Sıfırlama**
-	Sistemde bulunan ve içerik yönetimi(CMS) içerisinde bulunmayan bütün medya dosyalarını hem veritabanından hemde dosya sisteminden temizler.

**7-) Tamamen Sıfırlama**
-	Popup içerisinde bulunan tüm seçeneklerin seçilmesi durumunda sistem tamamen sıfırlanır. Tamamen sıfırlanması demek 1-2-3-4-5-6 maddelerin tamamı ve Content klasörünün tamamının sıfırlanması anlamına gelmektedir.