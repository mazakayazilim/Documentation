---
layout: default
title: Garanti Sanal Pos Kurulumu
parent: Banka Ayarları
grand_parent: Ayarlar
nav_order: 1
---

# Garanti Sanal Pos Kurulumu

1. Garanti Paneline Banka tarafından verilen Kullanıcı Adı ve Şifre ile girilir.
2. Giriş yaptıktan sonra Yönetim sekmesine tıklanır.
3. Üst köşede yazılan Terminal No ve Üye iş yeri No bilgileri alınır.
4. Panelde **BusinessNo** -> _TerminalNo_, **BusinessId** -> _Üye iş yeri No_ bilgileri ile doldurulur.
5. Kullanıcı Tanımama kısmına gelip bir Api kullanıcısı (İş yeri kullanıcısı oluşturulmalı) ve bu kullanıcıya şifre verilmeli. Bu şifre panelde **BusinesPass** alanına girilecek.
6. Kullanıcı resetleme kısmına gelerek PROVOUT kullanıcısına hatırlayabileceğiniz ÖRN: Modül.1235 gibi bir şifre belirlemelisiniz.
7. Son olarak Garanti Sanal Pos panelinde _3d Secure Key_ değiştirme alanına gelip Garanti Sanal Pos dokümanındaki 3d\_hesaplama.exe den 24 karakterli bir gelişigüzel karakterler girip (Modül1235Modülmodül) bunu hex olarak çevirip Garanti Sanal Pos ekranındaki Security Key değiştirme alanına girip hem de panelde Business Key alanına girmelisiniz. Model olarak ise 3D olarak veri tabanından yapmalısınız.

## Olası Hatalar

1. Eğer **TerminalId** tanımsız diyorsa; **BusinessNo** alanına _Üye İşyeri No_&#39;sunu girmişsinizdir.
2. Güvenlik kodu hatalı derse; **SecurityKey** alanınındaki şifreyi Garanti Sanal Pos ekranına girip tekrar değiştirmeniz ve bunu panelde **BusinessKey** alanına girmeniz gerekmektedir.