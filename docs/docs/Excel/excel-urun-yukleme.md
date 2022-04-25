---
layout: default
title: Excel Ürün Yükleme
description: "Mazaka Yazilim Eticaret dokumantasyonu."
permalink: /docs/excel-urun-yukleme
grand_parent: Excel
nav_order: 1
---

# Excel Kullanım Dökümantasyonuna Hoş Geldiniz!

Merhaba! burada exceli nasıl kullanacağını ve neler yapabileceğini öğreneceksin. Hazırsan başlayalım..

# Excel Çıktısı Alma

Panel üzerinde  **Toplu Güncelleme** > **Toplu Ürün Listesi Alma** seçeneği altından bulabilirsin. Sayfa açıldıktan sonra..
>Soldaki filtreleme menüsünden dolduruğun alanlarla eşleşen ürünlerin çıktısını alacaksın! Eğer doldurmazsan tüm ürünleri alacaksın, ürün sayısına ve seçim yaptın alan sayısına göre bekleme sürek exponansiyel olarak artacaktır! seçim yaparken çok beklemek istemiyorsan, dikkatli olmalısın. 
>
>Sağdaki alanda ise, hızlıca seçebilmen için senin için hazırlanmış, hızlıca güncelleme yapoabilmeni sağlayacak templateleri yada **diğer güncellemeler** alanından istediklerini seçerek,

excel ile çıktı al butonundan, verilerini elde edebilirsin.

## Ekleme, Güncelleme ve Silme İşlemleri Hakkında Bilmen Gerekenler
Excel ile sisteme aktarmak istediğin ürün listesinde;
- Eğer Id alanı boş ise bu ürün yeni ekleniyor demektir. Code alanı boş ise sistem 6 haneli bir kod atayacaktır.
- Eğer Id alanı dolu ise;
-- Code alanında -1 yazıyorsa silinecek,
--Kendi kodu yazıyor ise güncellenecek

demektir.  

Not: -1 yazdığınız halde ürün silinmemiş ancak kod alanı -1 olarak güncellenmiş ise bu demektir ki ürün, ana varyant ürünüdür alt varyantlar silinmeden, onu silemeyeceğiniz manasına gelir.

Giriş yapılan alanlara girilebilecek olası girilebilecek yanlış veriler için(fiyata alanında beşyüz yazmak gibi) elimizden gelen kontrolleri sağladık, sizde dikkatli olursanız seviniriz..

## Temel Ürün Ekleme/Güncelleme

Ürünlerinin sistemimize kayıt biçimi basitçe ürüne sadece bir defa yazabileceğin alanlar direkt olarak ürün tablosunda, birden çok defa ekleyebileceğin alanlar ayrı ek tablolarda tutulmaktadır. Bunlara örnek vermek gerekirse ürünün adı, dili gibi bir defa olan özellikler ile ürünün resimleri, varyantları, role göre fiyatlandırmaları gibi alanlar farklı tabloalarda olacaktır.


Temel ürün güncelleme olarak direkt ürün tablosunda yapacağınız güncellemeler olacaktır. Bu alanları excel çıktısı alırken seçtiğiniz takdirde, stunlarda göreceksiniz. Exceldeki alanları doldurduktan sonra işleminiz gerçekleşecektir.

## Yan Tablolarda Tutulan Alanların Güncellenmesi

Kategori, marka, role göre fiyatlandırma, etiket, opsiyonlar gibi alanların eklenirken yada güncellenirken dolu olması halinde eski verileri silip girmiş olduğunuz verileri kabul etmek yerine girdiğiniz her veriyi eğer daha önce eklenmemiş ise kaydediyoruz.
Bu size hızlı bir güncelleme imkanı sağlıyor, aksi halde 10 etiketi olan bir ürüne 11.etiket eklemek istediğinde, etiket alanına 11 tane veri yazmanız gerekmektedir. Dezavantajı ise varolan özellikleri silmek için ek bir işlem yapmanız gerekecektir.

**Kategori ->** alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!

 **Marka->** alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!
 
**Etiket->** alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!

**Dil->** alanına yazacağınız verileri noktalı virgül ile ayırarak yazmanız gereklidir!

**Opsiyon->** alanına yazacağınız veriler için **option1** ve **optiondeger1** şeklinde birbirini takip eden bir kural kullanmak zorundasın! Girmek istediğin ilk opsiyonu **option1** alanına ve değerini de **optiondeger1** alanına yazmalısın aksi halde hata alacaksın! devam eden opsiyonların için **option2** ve **optiondege2** şeklinde yazarak gerekli sayıda giriş yapabilirsin. Sırasını karıştırmamaya dikkat etmelisin!

**Rol Fiyat->** alanına yazacağınız veriler için **tprole1** , **tpprice1** ve **tpquantity1** şeklinde girişini kullanmak zorundasın. Alanlara ekleme yapacaksan bu alanların excel stunlarında bulunması zorunludur! eklemek istediğin diğer rol fiyatları için opsiyondaki gibi aynı alanların sonunda 2 yazarak yeni stunlara ekleyebilirsin. Sırasını karıştırmamaya dikkat etmelisin! Ürüne girmiş olduğun role ile ekli bir fiyat var ise güncelleme işlemi yapacaktır. Yok ise role ve ürüne o fiyat eklenecektir.
 
