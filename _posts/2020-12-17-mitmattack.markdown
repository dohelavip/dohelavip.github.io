---
layout: post
title:  ORTADAKİ ADAM (MITM) SALDIRISI
date:   2020-12-17 20:45:55 +0300
image:  01.jpg
tags:   [linux]
---
## Ortadaki Adam Saldırısı Nedir? 

Ortadaki adam saldırısı, kötü niyetli bir oyuncunun kendisini iki taraf arasındaki bir konuşmaya dahil ettiği, her iki tarafı taklit ettiği ve iki tarafın birbirine göndermeye çalıştığı bilgilere erişim sağladığı bir tür siber saldırıdır. 

Ortadaki adam saldırısı, kötü niyetli bir aktörün, dışarıdan herhangi biri çok geç olana kadar bilmeden, başka biri için tasarlanmış veya hiç gönderilmesi amaçlanmamış verileri durdurmasına, göndermesine ve almasına olanak tanır. 

Ortadaki adam saldırıları, MITM, MitM, MiM veya MIM dahil olmak üzere birçok şekilde kısaltılabilir.

![]({{site.baseurl}}/img/04.jpg)

* Ortadaki adam, kötü niyetli bir aktör kendisini insanlar veya sistemler arasındaki bir iletişim oturumuna aktarıcı / vekil olarak eklediğinde ortaya çıkan bir tür gizli dinleme saldırısıdır.
* Bir MITM saldırısı, işlemlerin, konuşmaların veya diğer verilerin aktarımının gerçek zamanlı işlenmesinden yararlanır.
* Ortadaki adam saldırıları, saldırganların çok geç olana kadar dışarıdan hiçbir tarafın haberi olmadan kendileri için olması amaçlanmamış verileri kesmesine, göndermesine ve almasına olanak tanır.

## Ortadaki Adam Saldırı Örnekleri 

![]({{site.baseurl}}/img/10.jpg)

Yukarıdaki görselde, saldırganın kendisini istemci ile sunucu arasındaki trafik akışı arasına soktuğunu fark edeceksiniz. 
Artık saldırgan, iki uç nokta arasındaki iletişime izinsiz girdiğine göre, yanlış bilgi enjekte edebilir ve aralarında aktarılan verileri yakalayabilir.

Aşağıda ortadaki adam kendisini soktuktan sonra neler olabileceğine dair başka bir örnek var.

![]({{site.baseurl}}/img/11.jpg)

Bilgisayar korsanı, fonlara erişmek için konuşmanın her iki tarafını da taklit ediyor. Bu örnek, bir istemci ve sunucuyla yapılan görüşmelerin yanı sıra kişiden kişiye konuşmalar için de geçerlidir. 
Yukarıdaki örnekte, saldırgan bir açık anahtarı ele geçirir ve bununla, insanları her iki tarafta da kandırmak için kendi kimlik bilgilerini, birbirleriyle güvenli bir şekilde konuştuklarına inanmaya dönüştürür.

## MITM Saldırılarına Duyarlı Etkileşimler

* Finansal siteler - oturum açma ve kimlik doğrulama arasında
* Genel veya özel anahtarlarla güvence altına alınması amaçlanan bağlantılar
* Oturum açma gerektiren diğer siteler - erişime sahip olarak kazanılacak bir şeyin olduğu yerler

## Diğer Oturum Kaçırma Biçimleri

Ortadaki adam, bir oturum kaçırma biçimidir. Ortadaki adam'a benzer diğer oturum kaçırma biçimleri şunlardır:

* Sidejacking - Bu saldırı, oturum çerezlerini çalmak ve bir kullanıcının oturumunu ele geçirmek için veri paketlerinin koklanmasını içerir. Bu çerezler, site güvenli olsa bile şifrelenmemiş giriş bilgileri içerebilir.

* Evil Twin - Bu, yasal bir ağ gibi görünen hileli bir Wi-Fi ağıdır. Kullanıcılar farkında olmadan hileli ağa katıldıklarında, saldırgan bir ortadaki adam saldırısı başlatarak sizinle ağ arasındaki tüm verileri yakalayabilir.

* Koklama - Bu, cihazınızdan veya cihazınıza gönderilen verilere müdahale etmek için hazır yazılımları kullanan kötü niyetli bir aktörü içerir.