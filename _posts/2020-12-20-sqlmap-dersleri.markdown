---
layout: post
title:  SQLMAP Giriş 
date:   2020-12-20 23:50:30 +0300
image:  sqlmapon.jpg
tags:   linux
---
## SQLMAP Giriş
Sqlmap, Kali linux içerisinde ki en <b>Sql Injection</b> aracıdır diyebiliriz. Birçok veritabananına uygun çalışma şekilleri ve 
<b>bypass</b> yöntemleri vardır. Ayrıca hızlı yapısı sayesinde oldukça ilgi görmekte. <b>Python</b> programlama dili ile yazıldığı için yapısını da inceleyebilirsiniz.
<b>Wireshark</b> gibi araçlar ile de <b>sql injection</b> esnasında <b>sqlmap</b> aracının gönderdiği sorgulara bakıp farklı şeyler öğrenebilirsiniz. 

![]({{site.baseurl}}/img/sqlmap.jpg)

Konsola "sqlmap -h" yazarak parametreleri görebilirsiniz. Ayrıca <b>sqlmap</b> aracını da anonim taramalarda gerçekleştirebilirsiniz.
<b>Proxy</b> ve <b>tor</b> desteği ile kolayca bu tür anonim işlemleri gerçekleştirebilirsiniz. Lakin unutulmamalı ki bu tür 
özellikler <b>Sql Injection</b> atağının uzun sürmesine neden olacaktır.
### Komutlar

<div class="table-container">
  <table>
    <tr><th>Komutlar</th><th>Açıklama</th></tr>
    <tr><td>-h,--help</td><td>Yardım menüsünü açar.</td></tr>
    <tr><td>-hh</td><td>Gelişmiş yardım menüsü.</td></tr>
    <tr><td>--version</td><td>Versiyon Öğrenme.</td></tr>
    <tr><td>-v VERBOSE</td><td>Gösterim şekli leve: 0-6 (varsayılan 1).</td></tr>
    <tr><td>-u URL,--url=URL</td><td>Hedef URL (e.g "http://www.site.com/vuln.php?id=1").</td></tr>
    <tr><td>-g GOOGLEDORK</td><td>Google Dork taraması yapar ve url adreslerini listeler.</td></tr>
	<tr><td>--data=DATA</td><td>POST işlemlerde data belirlemek için kullanılır.</td></tr>
	<tr><td>--cookie=COOKIE</td><td>COOKIE belirtmek için kullanılır.</td></tr>
	<tr><td>--random-agent</td><td>Rastgele HTTP User-Agent başlık bilgisi kullanmak için kullanılır.</td></tr>
	<tr><td>--proxy=PROXY</td><td>Rastgele proxy kullanmak için kullanılır.</td></tr>
	<tr><td>--tor</td><td>Tor Network ile tarama yapar.</td></tr>
	<tr><td>--check-tor</td><td>Tor doğruluk testi için kullanılır.</td></tr>
	<tr><td>--level=LEVE</td><td>Test seviyesi belirtmek (1-5, varsayılan 1).</td></tr>
	<tr><td>--risk=RISK</td><td>Risk seviyesi belirtme (0-3, varsayılan 1).</td></tr>
	<tr><td>--technique=TECH</td><td>Sql Injection Teknikleri belirme (varsayılan "BEUSTQ").</td></tr>
	<tr><td>-a,--all</td><td>Veri çekmek için kullanılır.</td></tr>
	<tr><td>-b,--banner</td><td>Database banner gösterir.</td></tr>
	<tr><td>--current-user</td><td>Database içerisindeki kullanıcıları listeler.</td></tr>
	<tr><td>--current-db</td><td>Genel database'yi gösterir.</td></tr>
	<tr><td>--passwords</td><td>Database'deki şifreleri çeker.</td></tr>
	<tr><td>--tables</td><td>Database'deki tabloları listeler.</td></tr>
	<tr><td>--columns</td><td>Database içerisindeki tabloların kolonlarını listeler.</td></tr>
	<tr><td>--schema</td><td>Database'leri listeler.</td></tr>
	<tr><td>--dump</td><td>Database'deki tablo girdilerini çeker.</td></tr>
	<tr><td>--dump-all</td><td>Bütün tablo girdilerini çeker.</td></tr>
	<tr><td>-D DB</td><td>Database belirtmek için kullanılır.</td></tr>
	<tr><td>-T TB</td><td>Tablo belirtmek için kulanılır.</td></tr>
	<tr><td>-C COL</td><td>Kolon belirtmek için kullanılır.</td></tr>
	<tr><td>--os-shell</td><td>Shell oturumu başlatır.</td></tr>
	<tr><td>--os-pwn</td><td>Meterpreter Shell başlatır.</td></tr>
	<tr><td>--tamper</td><td>Bypass Script'i kullanmak için kullanılır.</td></tr>
  </table>
</div>

Yukarıda çoğu komutun basit Türkçe açıklamasını görebilirsiniz.<b>Sqlamp</b> aracında komutların çoğu birbiriyle entegreli
bir biçimde kullanılmaktadır. Yani bir tablodan kolon çekerken tabloyu belirtmemiz gerekir gibi.

Devamı 2. Konuya beklemede kalın...