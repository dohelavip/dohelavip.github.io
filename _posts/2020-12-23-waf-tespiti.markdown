---
layout: post
title:  WAF (Web Application Firewall) Tespit
date:   2020-12-23 16:04:00 +0300
image:  waf.jpg
tags:   linux
---
Web Uygulama güvenlik duvarı tespiti aslında bilgi toplama aşamalarının başında gelmektedir. Bu sayede işleyişimize bir yön vermiş oluruz.
Yani <b>Firewall</b> olmayan bir sisteme yapılan işlemlerin bazıları başarısız olmaktadır. Bu nedenle bu taramayı yapmamız büyük önem taşır.

![]({{site.baseurl}}/img/wafw00f.jpg)

Bu taramayı bir araç ile rahatça yapabiliriz. <b><t>"wafw00f"</b></t> aracı belirli <b>firewall</b> sistemlerini belirlediğimiz <b>url</b>'ler üzerinde taramaktadır.

![]({{site.baseurl}}/img/wafw00f-l.jpg)

Konsola <b><t>"wafw00f -l"</b></t> yazarak hangi <b>firewall</b> sistemlerini tespit edebildiğini görebilirsiniz.
Toplam 120-130 adet sistemi tespit edebiliyor. En bilindik <b>ModSecurity</b> gibi sistemleri de test edebilir. Teset edeceğiniz firmada örnek olarak; <b>Sql injection</b> açığı tespit ettiniz ve sızma işlemine geçiyorsunuz.
Sql injection denemelerinde eğer engeller ile karşılaşıyorsanız, öncelikle bu araç ile sistemin ne tür bir <b>firewall</b> ile korunduğunu tespit edebilirsiniz.

![]({{site.baseurl}}/img/waftarama.jpg)

Taramamızı <b><t>"wafw00f www.siteadi.com"</b></t> şeklinde gerçekleştirdik. Görüldüğü gibi sonuç olarak <b>"Citrix NetScaler"</b> yazılımı ile sitenin korunduğu 
görülüyor. Böylelikle basit bir şekilde taramamızı gerçekleştirebiliriz.