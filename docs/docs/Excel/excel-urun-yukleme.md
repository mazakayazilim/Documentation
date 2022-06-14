---
layout: default
title: Excel İle İşlemler
description: "Mazaka Yazilim E-Ticaret Excel Yonetim Dokumantasyonu."
nav_order: 4
has_children: false
permalink: /docs/excel-urun-yukleme
---

# Excel Kullanım Dökümantasyonuna Hoş Geldiniz!

Merhaba! burada exceli nasıl kullanacağını ve neler yapabileceğini öğreneceksin. Hazırsan başlayalım..

# Excel Çıktısı Alma

Panel üzerinde  **Toplu Güncelleme** > **Toplu Ürün Listesi Alma** seçeneği altından bulabilirsin. Sayfa açıldıktan sonra..
>Soldaki filtreleme menüsünden dolduruğun alanlarla eşleşen ürünlerin çıktısını alacaksın! Eğer doldurmazsan tüm ürünleri alacaksın, ürün sayısına ve seçim yaptın alan sayısına göre bekleme süresi artacaktır! seçim yaparken çok beklemek istemiyorsan, dikkatli olmalısın. 
>
>Sağdaki alanda ise, hızlıca güncellemek istediğin alanları seçebilmen için hazırlanmıştır, güncelleme yapabilmeni sağlayacak templateleri yada **diğer güncellemeler** alanından istediklerini seçerek, güncellencek ürünlerin bu alanlarının çıktısını alacaksın.

excel ile çıktı al butonundan, verilerini elde edebilirsin.

## Ekleme, Güncelleme ve Silme İşlemleri Hakkında Bilmen Gerekenler
Excel ile sisteme aktarmak istediğin ürün listesinde;
- Eğer Id alanı boş ise bu ürün yeni ekleniyor demektir. Code alanı boş ise sistem 6 haneli bir kod atayacaktır.
- Eğer Id alanı dolu ise;
-- Code alanında -1 yazıyorsa silinecek,
--Kendi kodu yazıyor ise veya boş ise güncellenecek

demektir.  

**Not:** -1 yazdığınız halde ürün silinmemiş ancak kod alanı -1 olarak güncellenmiş ise bu demektir ki ürün, ana varyant ürünüdür alt varyantlar silinmeden, onu silemeyeceğiniz manasına gelir.

Giriş yapılan alanlara girilebilecek olası girilebilecek yanlış veriler için(fiyata alanında beşyüz yazmak gibi) elimizden gelen kontrolleri sağladık, sizde dikkatli olursanız seviniriz..

## Ürün Ekleme/Güncelleme

Ürünlerinin sistemimize kayıt biçimi basitçe ürüne sadece bir defa yazabileceğin alanlar direkt olarak ürün tablosunda, birden çok defa ekleyebileceğin alanlar ayrı ek tablolarda tutulmaktadır. Bunlara örnek vermek gerekirse ürünün adı, dili gibi bir defa olan özellikler ile varyantları, role göre fiyatlandırmaları gibi alanlar farklı tablolarda olacaktır.


Temel ürün güncelleme olarak direkt ürün tablosunda yapacağınız güncellemeler olacaktır. Bu alanları excel çıktısı alırken seçtiğiniz takdirde, stunlarda göreceksiniz. Exceldeki alanları doldurduktan sonra işleminiz gerçekleşecektir. Güncellemek isteyebileceğiniz temel alanların excelde stun adlarını aşağıda paylaşıyor olacağım

**Id:** Id

**Kodu :** Code 

**Aktif :** Active, atanabilecek değer (True/False) 

**Adı:** Name, atanabilecek değer (ürün adı)

**Link :** NormalizedName, atanabilecek değer (ürün adı linki)

**Para Birimi :** Currency, atanabilecek değer (TL,EUR,USD)

**Fiyat :** Price, atanabilecek değer (1200,50)

**İndirimli Fiyat :** PriceWithDiscount, atanabilecek değer (500)

**İndirim Ayarı :** UsePercentage, atanabilecek değer (1/0)

**Satışa Kapalı :** ClosedForSale, atanabilecek değer (True/False)

**Stok :** StockQuantity, atanabilecek değer (10)

**Marka :** Brand, atanabilecek değer (marka)

**Barkod :** Barcode, atanabilecek değer (barkod)

**Barkod2 :** Barcode2, atanabilecek değer (barkod2)

**N11 Fiyatı:** N11Price, atanabilecek değer (1000)

**N11 Transfer :** N11Transfer, atanabilecek değer (True/False)

**GG Fiyatı :** GGPrice, atanabilecek değer (300)

**GG Transfer :** GGTransfer, atanabilecek değer (True/False)

**HB Fiyatı :** HBPrice, atanabilecek değer (250,69)

**HB Transfer :** HBTransfer, atanabilecek değer (True/False)

**HBSKU :** HBSKU, atanabilecek değer (hbsku)

**Fiyat Gizle :** HidePrice, atanabilecek değer (True/False)

**Vergi :** Tax, atanabilecek değer (50)

**Vergi Dahil:** TaxIncluded, atanabilecek değer (True/False)

**Kısa Açıklama :** ShortDescription, atanabilecek değer (kısa açıklama)

**Açıklama :** Description, atanabilecek değer (açıklama)

**Açıklama2 :** Description2, atanabilecek değer (2.açıklama)

**Derinlik :** Depth, atanabilecek değer (30)

**Boy :** Height, atanabilecek değer (150,5)

**Ağırlık :** Weight, atanabilecek değer (23,7)

**Genişlik :** Width, atanabilecek değer (30)

**Seo Anahtar Kelime :** MetaKeyword, atanabilecek değer (metakeyword)

**Seo Açıklama :** MetaDescription, atanabilecek değer (metadescription)

**Seo Başlık :** MetaTitle, atanabilecek değer (metatitle)

**Arama Kelimesi :** SearchKeywords, atanabilecek değer (ürünle alakalı arama kelimeleri)

**Stok Bitince Satışa Kapat :** ClosedForSaleIfOutOfStock, atanabilecek değer (True/False)

**Stok Azalınca Uyarı Sınırı :** NotifyForStockQuantityBelow, atanabilecek değer (5)

**Eskileri Göster :** ShowOldReview, atanabilecek değer (True/False)

**Görünüm Sırası :** DisplayOrder, atanabilecek değer (1)

**Xml Ürün Kodu :** XmlProductCode

**Xml Ürün Kodu 2 :** XmlProductCode2

**Xml Ürün Kodu 3 :** XmlProductCode3




## Yan Tablolarda Tutulan Alanların Güncellenmesi

Kategori, marka, role göre fiyatlandırma, etiket, opsiyonlar gibi alanların eklenirken yada güncellenirken dolu olması halinde eski verileri silip girmiş olduğunuz verileri kabul etmek yerine girdiğiniz her veriyi eğer daha önce eklenmemiş ise kaydediyoruz.
Bu size hızlı bir güncelleme imkanı sağlıyor, aksi halde 10 etiketi olan bir ürüne 11.etiket eklemek istediğinde, etiket alanına 11 tane veri yazmanız gerekmektedir. Dezavantajı ise varolan özellikleri silmek için ek bir işlem yapmanız gerekecektir.

**Kategori :** Category, alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!

 **Marka :** Brand, alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!
 
**Etiket :** Tag, alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!

**Dil :** Culture, alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!

**Opsiyon :** alanına yazacağınız veriler için **option1** ve **optiondeger1** şeklinde birbirini takip eden bir kural kullanmak zorundasın! Girmek istediğin ilk opsiyonu **option1** alanına ve değerini de **optiondeger1** alanına yazmalısın aksi halde hata alacaksın! devam eden opsiyonların için **option2** ve **optiondeger2** şeklinde yazarak gerekli sayıda giriş yapabilirsin. Sırasını karıştırmamaya dikkat etmelisin!

**Varyant :** alanına yazacağınız veriler için **variant1** ve **variantdeger1** şeklinde birbirini takip eden bir kural kullanmak zorundasın! Girmek istediğin ilk varyantı **variant1** alanına ve değerini de **variantdeger1** alanına yazmalısın aksi halde hata alacaksın! devam eden varyantların için **variant2** ve **variantdeger2** şeklinde yazarak gerekli sayıda giriş yapabilirsin. Sırasını karıştırmamaya dikkat etmelisin!

**Rol Fiyat :** alanına yazacağınız veriler için **tprole1** , **tpprice1** ve **tpquantity1** şeklinde girişini kullanmak zorundasın. Alanlara ekleme yapacaksan bu alanların excel stunlarında bulunması zorunludur! eklemek istediğin diğer rol fiyatları için opsiyondaki gibi aynı alanların sonunda 2 yazarak yeni stunlara ekleyebilirsin. Sırasını karıştırmamaya dikkat etmelisin! Ürüne girmiş olduğun role ile ekli bir fiyat var ise güncelleme işlemi yapacaktır. Yok ise role ve ürüne o fiyat eklenecektir.
 
 
 
## Üründen Özellik Silme

Ürünlerine eklemiş olduğunuz marka, kategori, varyant gibi özellikleri nasıl sileceğinizi buradan okuyabilirsiniz.


**Kategori :** Category, alanına yazacağınız verilerden silmek için olanın önüne - ekleyin. Örnek     - kategori1

**Marka :** Brand, alanına yazacağınız verilerden silmek için olanın önüne - ekleyin. Örnek     - marka1
 
**Etiket :** Tag, alanına yazacağınız verilerden silmek için olanın önüne - ekleyin. Örnek     - etiket1

**Opsiyon :** alanına yazacağınız verilerden silmek için olanın değerinin önüne - ekleyin. Örnek **option1** ve **optiondeger1** alanları için kumaş rengi option1 alanında yazılıyken - kırmızı değerini optiondeger1 alanına girerseniz üründen kırmızı opsiyonu silinecektir.

**Varyant :** Varyant silmek için daha önce eklediğiniz ürün varyant ürün olarak üretilmiştir, üretilmiş olan varyant ürünün **Code** alanına -1 yazmanız gereklidir.
