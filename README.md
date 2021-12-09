# Documentation

## Altyapı

Dokümantasyon altyapısı için [Github Pages](https://pages.github.com/) altyapısını kullanıyoruz. Github Pages Markdown dosyalarını [Jekyll](https://jekyllrb.com/) ile statik websitelerine otomatik olarak dönüştürüyor. Bunun için https://github.com/mazakayazilim/Documentation reposunu kullanacağız.
Bu repo içerisine Markdown dosyalarını commit atmamız yeterli.

Dokümantasyon hazırlamak için Markdown formatını kullanacağız.

Markdown hakkında daha fazla bilgi almak için şuraya bakabilirsiniz: https://tr.wikipedia.org/wiki/Markdown

Markdown ile doküman hazırlamak için şu tarz bi editör kullanabilirsiniz : https://stackedit.io/app#

## Yeni sayfa nasıl eklenir?
Yeni bir sayfa eklemek için ilgili klasörü belirleyip içerisine eklediğiniz .md uzantılı bir dosya eklemeniz gerekmektedir. Dosya içerisine Markdown ile hazırlamış olduğumuz yazıyı ekliyoruz.

Yazının en başına şu alanlarını ekliyoruz:

```
---
layout: default
title: Sayfa Başlığı
description: "Mazaka Yazılım Eticaret dokümantasyonu."
permalink: /sayfa
parent: Ürün Sayfa
grand_parent: Ayarlar
nav_order: 1
---
```
layout -> hangi temayı kullanacağını belirtmek için. Şimdilik tek bir tema olduğu için default yazmamız yeterli.

title -> Hem sayfa başlığında hem menülerde kullanılan Başlık alanı

description -> Sayfa için açıklama alanı

permalink -> Sayfa için kullanılacak Url

parent -> Bir üst sayfayı belirtmek için kullanılan alan

grand_parent -> Menü hiyerarşisinde iki kademeli bir hiyerarşi kullanacaksak eklememiz gereken alan. En üst Sayfayı belirtmek için kullanılır.

nav_order -> Menüde sayfanın sırasını belirlemek için kullanılan alan.

Bu alanlardan gerekli olanları ekledikten sonra yeni bir commit atmamız yeterli. Bir kaç dakika sonra otomatikmen sisteme yansıyacaktır




