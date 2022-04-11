---
layout: default
title: Log Yonetimi
description: "Mazaka Yazilim E-Ticaret Log Yonetim Dokumantasyonu."
nav_order: 1
has_children: false
permalink: /docs/log-yonetimi
---

# Log Yönetimi Kullanım Dokümantasyonu

Merhabalar bu dokümantasyonda panel üzerinden nasıl bir sistemin log yönetimin yapıldığı inceleyeceğiz.

# Log Yönetimi


İlk olarak panel üzerinde bulunan sol menüden **Sistem** > **Ayarlar** seçeneklerine ulaşıyoruz. Daha sonra önümüze çıkan sayfada Log ile alakalı 3 adet ayar bulunmaktadır.

- '**Log Aç/Kapat'** ayarı sistemin bütün log mekanizmalarını kapatıp açmaya yaramaktadır.

- '**Dosya Log Aç/Kapat'** sadece dosyaya yazılan log ları kapatıp açmaktadır.

- '**Loki Log Aç/Kapat'** ise Loki sistemine log gönderip gönderilmeyeceğine karar verdiğimiz ayardır.

  

Yukarıdaki ayarları sistemin gereksinimlerine göre düzenleyebiliriz. Örneğin sadece dosyaya log yazmak istiyorsak

Log Aç/Kapat ve Dosya Log Aç/Kapat ayarının 'True' olması yeterlidir.

  

**Önemli**

Eğer ayarlar gözükmüyorsa log mekanizmasının çalışılması istenilen veritabanına bu 3 ayar eklenmelidir.

  

**1-) Log Görüntüleme**

Sistemlerin Loglarını görüntüleyebilmek için ortak platform olan log.mazakayazilim.com:3000 adresine giriş yapmamız gerekmektedir. Giriş bilgileri;

-  **Kullanıcı Adı** : admin

-  **Şifre**: 238855Yby.

  

- Giriş yaptıktan sonra karşımıza 'Welcome to Grafana' yazılı bir ekran çıkmaktadır. Daha sonra sol tarafta bulunan butonlarda pusula işaretine(Zil işaretinin üzerindeki) tıklıyoruz. Tıkladıktan sonra bizi aşağıdaki ekran karşılamakta. Burada 'Explore' yazan yerin yanındaki dropdrown'dan Loki'yi seçiyoruz.

![Loki Expolorer](https://i.ibb.co/DpKwXv8/image.png)

  

- Daha sonra sol üst tarafta bulunan 'Log browser' seçeneğine tıklıyoruz. Tıkladıktan sonra bize sistemin gönderdiğin log ların etiketlerini gösterecektir.

![Log Tags](https://i.ibb.co/XW95PDD/image.png)

- Bu etiketlerden en az bir tanesini (birden çok seçim yapılabilir) seçerek devam edebiliriz. Örnek olarak aşağıdaki görselde 'Application' etiketi altındaki 'MazakaCore' seçilmiştir.

![Select Tags](https://i.ibb.co/jJhyDKQ/00d22082-37df-43a6-839c-b32bd51aa07d.png)

- Etiket seçimi yapıldıktan sonra o etikete ait logların gelmesi için sağ üst tarafta bulunan 'Run query' butonuna tıklanabilir. Veya görseldeki gibi ne kadar sürede otomatik olarak log ları sorgulayacağını belirleyebiliriz. 5s,10s, 1m gibi. Loglar geldikten görselin alt tarafındaki gibi bir sonuç elde ediyoruz. Üzerine tıklayarak logun detayına ulaşabiliriz.

  

**Ekstra**

- https://sbcode.net/grafana/logql adresine girerek nasıl log query yazılacağını inceleyebilirsiniz.