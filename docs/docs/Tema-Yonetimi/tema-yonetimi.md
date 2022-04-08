---
layout: default
title: Tema Yonetimi
description: "Mazaka Yazilim E-Ticaret Tema Yonetim Dokumantasyonu."
nav_order: 1
has_children: false
permalink: /docs/tema-yonetimi
---

# Tema Yönetimi Kullanım Dökümantasyonu

Merhabalar bu dökümantasyonda panel üzerinden nasıl bir sistemin tema yönetimin yapıldığı inceleyeceğiz.  

# Tema Yönetimi

İlk olarak panel üzerinde bulunan sol menüden **İçerik Yönetimi** > **Sayfa Listesi** seçeneklerine ulaşıyoruz. Daha sonra önümüze çıkan sayfanın sağ üst tarafında yeşil renkte bulunan **Tema İşlemleri** butonuna tıklıyoruz ve karşımıza dropdrown çıkıyor.

Açılan dropdrown içerisinde 2 adet seçenek ile karşılaşıyoruz. Bu seçenekleri üzerine gelip tıklama işlemi gerçekleştirdiğimizde popup açılıyor ve seçtiğimiz seçeneğe göre bir ekran geliyor.

  

**1-) Tema Dışarı Aktar (Export)**

Tema dışarı aktar butonuna bastığımızda önümüze bu olayla alaklı bir poup açılmaktadır. Açılan popup içersinde 3 tane element bulunmakta. En soldaki tema seçimi, ortadaki eğer oluşacak dosyayı(zip) şifrelemek istiyorsak şifre ve en sağda da bir buton bulunmakta.  Butonun yanındaki aşağı ok işaretine bastığınızda karşınıza 2 seçenek çıkmakta.

- İlk seçenek dosya olarak indir seçeneği seçtiğiniz temayı, eğer şifre oluşturduysanız onunla beraber fiziksel bir dosya olarak bilgisayarınıza indirir.  **Dikkat** buradaki dosya içersine göz atarbilirsiniz fakat içersine müdahale ederseniz dosyayı tekrar yükleyemezsiniz.
- İkinci seçenek olarak ise link üret önümüze çıkmakta. Bu seçenekte yine seçilen tema ve şifre ile bir dosya oluşturur fakat bunu fiziksel olarak indirmeyerek sunucuya kayıt eder ve size bir link verir. Bunu ister indirebilirsiniz ister doğrudan temayı içeri aktar(Import) için kullanabilirsiniz.
 
**2-) Tema İçeri Aktar (Import)**

Tema dışarı aktar butonuna bastığımızda önümüze bu olayla alaklı bir poup açılmaktadır. Açılan popup içersinde 4 tane element bulunmakta. 
 - İlk olarak **Dosya Seç** alanı eğer fiziksel bir tema dosyası(zip) yüklemek istiyorsanız buraya tıklayarak cihazınızdan dosyayı seçebilirsiniz. 
- İkinci olarak eğer linkten dosya yüklemek istiyorsanız **Link Giriniz** alanına dosya uzantınızla beraber "http://domain/dosya_yeri/tema_isimi.zip" şeklinde girebilirsiniz. 
**Dikkat** eğer 2 alanı da doldurursanız öncelik olarak fiziksel dosya kabul edilecektir.
Dosya seçme veya link girme işleminiz yaptıktan sonra varsa dosyaya ait şifreniz onuda gerekli alana girerek **Teme İçeri Aktar** butonuna basmanız yeterlidir. 

**3-) Detaylar**

- Sistem içerisine birden fazla tema import edebilirsiniz fakat aktif olarak 1 tane kullanabilirsiniz.

- Tema export esnasında page sectionlar json olarak alınır daha sonra içersinde geçen fotoğraflar ve tema dosyaları zip olarak alınır.

- Tema import esnasında ise export sırasında json dosyası veritabanına işlenir, alınan fotoğraflar uploads dosyasına temalar ise themes dosyası içersine çıkarılır.

**Önemli**
 - Sisteminizdeki **Content** klasörüne izin vermeniz gerekmektedir.
