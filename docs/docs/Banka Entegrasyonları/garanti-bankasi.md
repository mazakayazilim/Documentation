---
layout: default
title: Garanti Bankası Sanal Pos Dokümanı
parent: Banka Entegrasyonu
nav_order: 1
---

# Garanti Bankası Sanal Pos Dokümanı

**1-)GİRİŞ YAP**
Garanti BBVA tarafından gelen kurulum mailinden GİRİŞ YAP butonuna tıklayın.

**1)** Garanti Paneline Bbanka tarafından verilen Kullanıcı Adı ve Şifre ile girilir.
**2)** Giriş yaptıktan sonra Yönetim sekmesine tıklanır.
**3)** Üst köşede yazılan **Terminal No** ve **Üye iş yeri No** bilgileri alınır.
**4)** Panelde **BusinessNo** > **Termianl No** ,  **BusinessId** > **Üye iş yeri No** bilgileri ile doldurulur.
**5)** Kullanıcı Tanımama kısmına gelip bir Api kullanıcısı(İş yeri kullanıcısı oluşturulmalı) ve bu kullanıcıya şifre verilmeli. Bu şifre panelde Busines Pass alanına girilecek.
**6)** Kullanıcı resetleme kısmına gelerek PROVOUT kullanıcısına hatırlayabileceğiniz ÖRN: Modül.1235 gibi bir şifre belirlemelisniz.

**7)** Son olarak Garanti Sanal Pos panelinde 3d secure Key değiştirme alanına gelip Garanti Sanal Pos dokümanındaki 3d_hesaplama.exe den 24 karakterli bir gelişigüzel karakterler girip(Modül1235Modülmodül) bunu hex olarak çevirip Garanti Sanal Pos ekranındaki Security key değiştirme alanına girip hem de panelde Business Key alanına girmelisiniz. Model olarak ise 3D olarak veritabanından yapmalısnız. 


**Sanal Pos Hataları**
**1-)** Eğer **TerminalId** tanımsız diyorsa; **Business No** alanına üye işyeri nosunu girmişsinizdir.
**2-)** Güvenlik kodu hatalı derse ; Security Key alanınındaki şifreyi Garanti Sanal Pos ekranına girip tekrar değiştirmeniz ve bunu panelde Business Key alanına girmeniz gerekmektedir.



