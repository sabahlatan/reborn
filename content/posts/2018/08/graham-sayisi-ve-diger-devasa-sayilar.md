---
title: "Graham Sayısı ve Diğer Devasa Sayılar"
date: "2018-08-14"
categories: 
  - "genel-kultur"
tags: 
  - "buyuk-sayi"
  - "buyuk-sayilar"
  - "devasa-sayilar"
  - "google"
  - "googol"
  - "googolplex"
  - "graham-sayisi"
  - "grahams-number"
  - "matematik"
  - "ok-gosterimi"
  - "us-kulesi"
---

İnsanlar günlük yaşantısında genellikle milyar üstü sayılarla pek uğraşmaz. Bu yüzden de trilyon ve sonrası çok karıştırılır. Ancak bilişim ve bilgisayar bilimlerinin uzantısı olan teknolojiler söz konusu olduğunda büyük sayılar günlük hayatın içine girmeye başlar. Bunun nedeni ise gelişen teknoloji ve sürekli olarak katlanan kapasitelerdir. Çünkü sınırlar mecburi olarak çok aşağıya konuldu, bit ve Byte bugün için çok küçük değerler. Her bir jenerasyonda hafıza birimleri, aktarım hızları, işlem güçleri bin katına çıkıyor. Bunlardan bahsetmek içinse doğrudan sayı isimleri kullanmak yerine kilo, mega, giga, tera gibi Yunanca kökenli önekler kullanılıyor. kilo bin, mega milyon, giga milyar, tera trilyon anlamlarına gelir. Bunların katları olan peta, eksa, zetta, yotta ise katrilyon, kentilyon, sekstilyon ve septilyon anlamlarına geliyor. Bilişimde dahi şu an için kolay kolay karşınıza çıkamayacak değerler. Fizik gibi çok büyük ve çok küçük boyutlarla uğraşılan alanlarda ise genellikle bilimsel gösterim kullanılır ve üslü sayılar daima önplanda olur.

Fakat bu yazıda bahsedilecek sayılar için tüm bu sayılar aslında çok küçük kalıyor. Öyle ki kimi zaman aşina olunan tüm sayısal gösteirm metodları dahi yetersiz kalıyor. Üslü sayılarla yalnızca 4 karakter kullanılarak dahi gözlemlenebilir evrendeki yaklaşık atom sayısını göstermek mümkün. Dolayısıyla üslü sayı sistemi de bir noktaya kadar büyük değerleri göstermek için oldukça yeterli bir potansiyele sahip. Bu yüzden Fizik gibi dallarda oldukça önemli bir noktaya sahipler.

Çok büyük sayıları göstermek için çeşitli notasyonlar kullanılır. Knuth yukarı ok gösterimi, Conway dizisi ok gösterimi, Steinhaus-Moser gösterimi, tetrasyon bunlardan bazılarıdır. Bizim burada en çok işimize yarayacak olanı Knuth yukarı ok gösterimi olacak.

İlk sayı olan **Googol** için bu gösterimlere ihtiyaç olmayacak, standart bir üs gösterimi yeterli. Google'ın isminin kökeni de olan bu sayı 10100'a eşit. Kısaca 1'in sağına eklenmiş 100 adet 0 demek. Fazla bir esprisi yok, uydurulmuş olmak için uydurulmuş bir sayı. 1 Googol değerine en yakın faktöriyel gösterim 70 faktöriyele ait. 70! yaklaşık 1.198 Googol'a eşit.

Googol'dan türetilen başka bir sayı var, bu sayının ismi ise **Googolplex**. Kısaca 10 üzeri Googol, yani 1'in yanına Googol kadar 0 eklenmesiyle bir Googolplex elde ediliyor. 10(10100) şeklinde gösterilebilir. Bu sayı gözlemlenebilir evrendeki atom miktarından çok daha büyük bir sayı. Gözlemlenebilir evrendeki atom miktarının yaklaşık 1080 civarında olduğu tahmin edilmekte.

Bu boş işler Googolplexian, Googolplexianth şeklinde devam ediyor. Herbiri bir öncekinin 10 üssü hali.

**Graham sayısı** şu an için bir anlamı olan en büyük sayı, Googol ve Googolplex'ten farklı olarak. Bunu belirtmek önemli, çünkü kimisi bunu 10'la çarpıp "bakın daha büyük bir sayı buldum, asıl beni sokun rekorlar kitabına" diyebiliyor. Akıl sağlığınızı korumak için Youtube ve Facebook yorumlarından uzak durun. Graham sayısı Ramsey teorisindeki problemler için üst sınır olan sayı. Daha önce bahsettiğim sayılarla kıyaslanamayacak kadar büyük. Evrendeki en küçük uzunluk birimi planck uzunluğu olarak görülüyor ve bu uzunluktan daha küçük boyutta fiziksel bir evrenin var olamayacağı düşünülüyor. Gözlemlenebilir evrendeki tüm planck uzunluklarına bu sayının bir hanesi yazılsaydı dahi, bu sayıyı açık halde göstermek için yetersiz kalacaktı. Fakat bu ve bunun gibi sayıları başlarda da bahsettiğim gibi çeşitli notasyonlarla göstermek mümkün. Graham sayısı için ise Knuth yukarı ok notasyonu kullanılıyor. Gereken tek sembol bu şekildeki gibi yukarı doğru uzanmış bir ok.

"**↑**"

Bu sembol aslında üs gösteriminin farklı bir şekli. Bu notasyonu şu şekilde tanıdık biçimlere dönüştürebiliriz.

3↑3 = 33 3↑↑3 = 3↑(33) = 3(33)

Graham sayısını gösterebilmek için birkaç adım gerekiyor.

Öncelikle 3↑↑↑↑3 ile başlıyoruz, arada 4 adet ok var. Bu gerçekten çok büyük bir sayı. Buna G1 diyelim.

G1 = 3↑↑↑↑3

Bir sonraki adım için iki adet 3'ün arasına G1'in büyüklüğü kadar ok koyuyoruz. Buna da G2 diyelim. Bu şekilde her adımda bir önceki adımdaki sayı kadar arada ok oluyor.

G64 adımında duruyoruz. Çünkü Graham sayısı G64 adımındaki sayı.

G1 = 3↑↑↑↑3 (4 ok) G2 = 3↑...↑3 (G1 kadar ok) G3 = 3↑...↑3 (G2 kadar ok) ... G64 = 3↑...↑3 (G63 kadar ok)

Graham sayısıyla ilgili olarak, eğer bir insan bu sayının gerçek anlamda büyüklüğünü düşünürse ve bunu başarırsa beynindeki küçük bir bölgesine bu kadar büyük bir bilgi sığdırdığı için beyninin karadeliğe dönüşeceği söylenir. Gerçekten de kendine özgü Schwarzschild yarıçapı boyutuna indirilen her varlık karadeliğe dönüşür. Graham sayısının gerçek büyüklüğünü kavrayabilecek nöron ve impuls miktarını hayal etmek demek Graham sayısının kendisini hayal etmekten çok da farklı değil.
