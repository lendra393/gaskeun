+++
author = "ligar"
bg_image = "/images/14.png"
categories = ["tes"]
date = 2020-11-13T17:00:00Z
description = "tes agc"
image = ""
tags = ["ewad"]
title = "COBA AGC DI SINI"
type = "post"

+++
StupitBotMOD + Arsae 2.0

UBAY GATES·MINGGU, 04 OKTOBER 2020·

Assalamualaikum sob, sehubungan dengan post ane disini [https://www.facebook.com/groups/stupidbotmod/permalink/649199709114124/](https://www.facebook.com/groups/stupidbotmod/permalink/649199709114124/ "https://www.facebook.com/groups/stupidbotmod/permalink/649199709114124/") ane mau berbagi pengalaman gimana caranya pasang kode Arsae 2.0 di StupidBotMOD yang unik ini :)

Langsung aja!

Pergi ke folder xxx\\themes\\z\\layouts\\partials

Edit file arsae-client.html, Isi dengan domain server Arsae ente, contoh:

<script type='text/javascript'>

//<!\[CDATA\[

if(document.referrer)

{

var cek = document.referrer;

var is_se = cek.includes('.google.') || cek.includes('.bing.') || cek.includes('yandex.') || cek.includes('facebook.') || cek.includes('pinterest.');

if(is_se)

{

var url = window.location.href;

window.location = "[https://domainarsae.com/?arsae=](https://domainarsae.com/?arsae= "https://domainarsae.com/?arsae=")"+ encodeURIComponent(url);

}

}

//\]\]>

</script>

Edit file ads-below-title.html dan ads-below-content.html, Isi dengan script iklan adsense ente, contoh:

<script async src="[https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js](https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js "https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js")"></script>

<ins class="adsbygoogle"

style="display:block; text-align:center;"

data-ad-layout="xxxxx"

data-ad-format="fluid"

data-ad-client="ca-pub-xxxxxxxxxxxxxx"

data-ad-slot="xxxxxxxxxxxxxxx"></ins>

<script>

(adsbygoogle = window.adsbygoogle || \[\]).push({});

</script>

Edit file ads-in-article1.html dan ads-in-article2.html, Isi dengan kode dibawah:

{{ printf "<!--ads/script-iklan-arsae.txt-->" | safeHTML }}

Untuk file stupidhugo-en\\engine\\recipe\\create\\content.html biarkan default

Selesai.

Cek di google dengan ketik site:[https://domianfirebase.web.app,](https://domianfirebase.web.app, "https://domianfirebase.web.app,") jika ter-redirect ke domainarsae.com dan iklan keluar saatnya gasspoll create content!