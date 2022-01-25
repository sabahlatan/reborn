---
title: "32-bit ve 64-bit İşlemci Arasındaki Fark Tam Olarak Nedir"
date: "2018-05-11"
categories: 
  - "teknoloji"
tags: 
  - "16-eb"
  - "16-exabyte"
  - "32-bit-islemci"
  - "32-bit-ve-64-bit-arasindaki-farklar"
  - "32-bit-vs-64-bit"
  - "4-gb-ram"
  - "64-bit-islemci"
  - "adresleme"
  - "bilgisayar"
  - "cpu"
  - "donanim"
  - "islemci"
  - "islemciler"
  - "ram"
thumbnail: "cpu.jpg"
---

32-bit işlemcilerin tarihi artık doldu ve yerini büyük oranda 64-bit işlemcilere bırakmaya başladı. Neden 32-bit'in artık eskimiş bir teknoloji olduğunu yazının sonuna doğru anlayacaksınız. Bu kadar fazla bahsedilen bir konu hakkında yazmamın nedeni, bu konuyla ilgili karşınıza çıkan kaynakların çoğunun yalan yanlış bilgilerle dolu olması. Kendileri tam olarak anlamadan anlatmaya çalıştığından dolayı internet çöp bilgilerle dolu.

32-bit ve 64-bit işlemcinin arasındaki farkın kolayca anlaşılamamasının nedeni isimlendirmedeki eksiklikten kaynaklanıyor. 32-bit bir işlemciden bahsedildiğinde akılda canlanan görsel işlemcinin her saat vuruşunda 32 bit veri işlediği veya işlemcinin az çok nasıl çalıştığını bilen biri için register denen hafıza alanlarında 32 bit veri tutulduğu olacaktır. Fakat 32-bit adreslemeli işlemci buna çok daha uygun bir isim.

Birçok kaynakta tamamen yanlış bir şekilde 64-bit işlemcilerin 32-bit işlemcilerden 2 kat daha hızlı olduğu söyleniyor. Kimileriyse biraz daha öğrenmiş veya uyarılmış olacak ki bu hızın 2 kat değil, çok daha fazla olduğunu söylüyor. Fakat gidip 32-bit işlemciyi tek şeritli, 64-bit işlemciyi çift şeritli otoyola benzetiyor. Bu kavram için çift şeritli yol benzetmesi hiçbir şekilde uygun ve doğru değil.

Şimdi teker teker açıklamaya başlayalım. Bilgisayarın birincil hafıza birimi olan RAM, sabit miktarda veri alabilen satırlara sahiptir. İşlemciler bu satırlara ulaşır, satırdaki ifadeleri alarak uygun işlemleri gerçekleştirir. Bu satırlarda buyruk adı verilen, işlemcinin hangi işlemleri yapacağını belirleyen en temel programlama ifadeleri veya direkt olarak veri bulunabilir. Doğal olarak her satırın bir adresi vardır ve işlemci bu adreslere erişir, buyruklara da bağlı olarak bu adresler üzerinde gidip gelir.

32-bit işlemcide 32 bit ile gösterilen adresleme kullanılır. 32 bit 232 tane adres gösterebilir, yaklaşık olarak 4 milyar. Bu da 4 GigaByte'lık bir hafızayı yönetebilir demek. Bu yüzden normal şartlar altında 32-bit bir işlemcinin olduğu bilgisayara maksimum 4 GB boyutunda bir RAM takılabilir. Öte yandan 64-bit bir işlemci ise 264 adres gösterebilir ki, bu da yaklaşık 16 ExaByte veri demek. Bu birim GigaByte'tan, onun 1024 katı olan TeraByte'tan ve onun da 1024 katı olan PetaByte'tan sonra gelir. Şimdiki teknolojiyle ulaşılması imkansız denebilecek bir değer. Kısaca hemen hemen IPv6 mevzusunda olduğu gibi, eski hesaplara göre kullanılmaya devam eden teknolojiler bugün sınıra dayanmış durumda ve yeni çıkan alternatifleri çok daha ulaşılmaz boyutlarda, en azından şimdilik.

Bu iki işlemci mimarisinin arasındaki farkı çok daha iyi anlatabilmek için bir kargo servisi örneği verilebilir. Adres kayıt sistemlerindeki kapı numarası basamak sayısı 2 ile sınırlı olan bir kargo firması olsun. Bu firmanın kaydedebileceği maksimum ev 0 dahil 100 adettir. Dolayısıyla verebileceği hizmet yalnızca bu 100 ev dahilindedir. Basamak sayısı 6'ya çıktığında ise hizmet verebileceği ev sayısı 1.000.000 olacaktır. Yani 3 katı değil, 100.000 katına çıkacaktır.

Konudan bağımsız olarak, 2 üssü şeklinde tanımlanan birimlerin GigaByte, MegaByte gibi isimler yerine GibiByte (GiB), MebiByte (MiB) şeklinde anılması gerektiğini, 10 üssüyle tanımlanan ifadelerin bu isimleri alması gerektiğini savunan bir görüş var. Daha sonra başka bir yazıda bir ihtimal bundan da bahsederiz.
