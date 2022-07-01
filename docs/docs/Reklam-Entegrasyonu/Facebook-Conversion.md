---
layout: default
title: Facebook Conversion API Entegrasyonu
description: "Mazaka Yazilim E-Ticaret sistemini kullanırken satışlarınızı ve ürün fiyatları üzerindeki hakimiyetinizi arttırmanız kullanabileceğiniz bir platform olan facebook business ile bağlantı kurulması ve reklam sisteminin yönetilmesi için gerekli dökümanlar."
nav_order: 4
has_children: false
permalink: /docs/Facebook-Conversion
---

# Facebook Conversion API Dökümantasyonuna Hoş Geldiniz!



Merhaba! burada facebook reklamların nasıl kullanacağını ve neler yapabileceğini öğreneceksin. Hazırsan başlayalım..



+ # 1. Kurulum



+ # 1.1 Business Hesabı Oluşturma
Öncelikle facebook hesabınızı **business** olarak ayarlamalısınız, bu işlem biraz zaman alabilir. 



+ # 1.2 Sitenizi Facebook'a Veri Kaynağı Olarak Ekleme
Facebook Business hesabınız oluştuktan sonra, **business.facebook.com** sayfasına giderek soldaki menüden Event Manager(Olay Yöneticisi) ne girmelisiniz.
![image alt ><](https://user-images.githubusercontent.com/63093864/176864198-910d15cd-7849-4aa2-b683-f156c08a033c.png)
 
 
 
Yine soldaki menüden Connect Data Source(Veri Kaynağı Bağla) seçeneği aldından sisteminizi, facebook business hesabınıza ekleyin. Soldaki menü altında yer alan Data Sources(Veri Kaynakları) kısmından eklemiş olduğunuz sisteminizi görüntüleyebiliyor olmanız gerekiyor.
![image alt ><](https://user-images.githubusercontent.com/63093864/176868111-e51abdf8-0abb-4fae-b158-937d76427361.png)



+ # 1.3 Coversion API Desteğini Aktif Etme
Buraya kadar ki aşamalar tamamladıktan sonra Settings(ayarlar) kısmından conversion api için key üretmeniz gerekmekte, üretme işlemini tamamladıktan sonra yönetim işlemlerini de Manage Integrations(Entegrasyonları Yönet) kısmından yapabilirsiniz.
![image alt ><](https://user-images.githubusercontent.com/63093864/176888018-7d3daa49-fa72-4465-ba70-a35729d7b382.png)



Settings menüsü altında biraz aşağılara gidince Turn on automatic advanced matching(Otomatik gelişmiş eşleştirmeyi aç) seçeneğini aktif etmelisiniz, bu seçenek gönderilecek verileri sisteminize eşleştirilmesini kolaylaştıracaktır. Altına açılan ok ile gelen seçeneklerden de müşterilerinizi hangi özellikleri ile eşleştirmek istiyorsanız onları seçebilirsiniz.
 ![image alt ><](https://user-images.githubusercontent.com/63093864/176888836-7734c70c-d386-470d-9298-4ba13f3f3981.png)



Biraz daha aşağı doğru gidince **Conversions API** sekmesini göreceksiniz. Burdaki Set Up Manually(Manuel Kurulum) altındaki Get Started(başla) seçeneği ile devam edelim.
![image alt ><](https://user-images.githubusercontent.com/63093864/176889037-4d4a036c-9cc3-402e-ac32-790c7cf49a4e.png)



Sizi yeni bir sayfaya yönlendirecektir.
![image alt ><](https://user-images.githubusercontent.com/63093864/176889339-d1a2bd56-2324-4bf8-8401-59d10e1c0e6e.png)


Continue(Devam et) diyerek sonraki sayfaya geçiyoruz, burada size uygun olan takip etmek istediğiniz seçenekleri işaretliyorsunuz.
![image alt ><](https://user-images.githubusercontent.com/63093864/176889766-f076a125-23f5-4cbf-85b3-279973575936.png)



Bir sonraki sayfada bu seçmiş olduğunuz eventlerin takip etmesini istediğiniz verileri seçeceksiniz. Burada bizim sistemimizle tam uyuşması bazı alanları kesinlikle işaretlemeniz gereklidir. Bu alanlar facebook tarafında hem mükerrer kayıt oluşmasını engelliyor, hem de bizim sistemin desteklerken verilerde hata yapmamasını sağlıyor.


**Zorunlu işaretlenmesi gereken alanlar** = Event ID, Currency, Value, Content IDs, Contents, Content Name, Order ID bu alanlardan bazıları seçtiğiniz evente göre değişiklik gösterebilir eğer yoksa işaretlemeyin.
![image alt ><](https://user-images.githubusercontent.com/63093864/176890570-69f99f7e-fa24-41a8-9b99-2a4ca717867a.png)


Bir sonraki ekran oluşturduğunuz eventleri incelemek ve doğru ise devam etmeniz için olacak, eğer değişiklik yapmak isterseniz sonrada buraya gelebiliyorsunuz(Manage Integrations). Diğer ekrandan da bitir diyerek kurulumu tamamlayın.



+ # 1.4 Coversion API Key Üretme
Manage Integrations tıklayarak açılan menüden Key üreteceğiz, dilerseniz eventleri tekrar ayarlamak için gireceğiniz yerde burasıdır.
![image alt ><](https://user-images.githubusercontent.com/63093864/176891009-c8c69603-643d-4e69-b3df-4b70cc863cdf.png)


Açılan pencereden Start Sending Events seçeneğini tıklayalım.
![image alt ><](https://user-images.githubusercontent.com/63093864/176891365-67fe0dc8-f515-4f8f-9b76-8615aba62977.png)

Ve buradan api için gerekli key üretimini yapalım
![image alt ><](https://user-images.githubusercontent.com/63093864/176891444-5c03ab27-0fa9-415b-b4e9-8d3a3c2e47b2.png)


 
 
 
 + # 2 Mazaka E-Ticaret Sistemine API Ekleme
Üretimiş olduğunuz tokeni sisteme girerek ve verileri facebooka gönder seçeneğini aktif ederek çalışmasını sağlayabilirsiniz.
