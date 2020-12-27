---
layout: post
title:  WAF (Web Application Firewall) Tespiti
date:   2020-12-23 16:04:00 +0300
cover:  assets/images/waf.jpg
tags:   linux
navigation: True
class: post-template
subclass: 'post'
author: dohela
---
Web Uygulama güvenlik duvarı tespiti aslında bilgi toplama aşamalarının başında gelmektedir. Bu sayede işleyişimize bir yön vermiş oluruz.
Yani <b>Firewall</b> olmayan bir sisteme yapılan işlemlerin bazıları başarısız olmaktadır. Bu nedenle bu taramayı yapmamız büyük önem taşır.

![]({{site.baseurl}}assets/images/wafw00f.png)

Bu taramayı bir araç ile rahatça yapabiliriz. <b>"wafw00f"</b> aracı belirli <b>firewall</b> sistemlerini belirlediğimiz <b>url</b>'ler üzerinde taramaktadır.

![]({{site.baseurl}}assets/images/wafw00f-l.png)

Konsola <b>"wafw00f -l"</b> yazarak hangi <b>firewall</b> sistemlerini tespit edebildiğini görebilirsiniz.
Toplam 120-130 adet sistemi tespit edebiliyor. En bilindik <b>ModSecurity</b> gibi sistemleri de test edebilir. Teset edeceğiniz firmada örnek olarak; <b>Sql injection</b> açığı tespit ettiniz ve sızma işlemine geçiyorsunuz.
Sql injection denemelerinde eğer engeller ile karşılaşıyorsanız, öncelikle bu araç ile sistemin ne tür bir <b>firewall</b> ile korunduğunu tespit edebilirsiniz.

![]({{site.baseurl}}assets/images/waftarama.png)

Taramamızı <b>"wafw00f www.siteadi.com"</b> şeklinde gerçekleştirdik. Görüldüğü gibi sonuç olarak <b>"Citrix NetScaler"</b> yazılımı ile sitenin korunduğu 
görülüyor. Böylelikle basit bir şekilde taramamızı gerçekleştirebiliriz.