---
title: "Kayıtlı Wi-Fi Şifresini Görüntülemek"
date: "2016-10-23"
categories: 
  - "android"
  - "teknoloji"
tags: 
  - "android"
  - "androidde-wifi-sifresini-gorme"
  - "ios"
  - "linux"
  - "mac-os"
  - "show-wifi-password"
  - "wifi"
  - "wifi-sifresini-goruntuleme"
  - "wifi-sifresini-gosterme"
  - "windows"
  - "windowsta-wifi-sifresini-gorme"
  - "wireless"
thumbnail: "2.jpg"
---

Teknolojinin ulaştığı noktanın etkisiyle kablosuz ağlara bağlanan cihazlar artık her evin dört bir köşesinde yer alıyor. İnsanlar artık kablosuz bağlantılar olmadan yaşayamaz halde. Tabii bu bağlanılan ağlar güvenlik anahtarı, yani ağa bağlanma şifresi kullandığında zaman içinde başka bir cihazı bu ağa bağlamak gerektiğinde unutulabiliyor.

Mevcut ağ ev tipi bir modem bağlantısı olduğunda ve ağ sahibi iken web tarayıcısı olan bir cihazla 192.168.1.1 şeklindeki adrese girerek modem arayüzüne bağlandıktan sonra şifreyi görmek ve değiştirmek mümkün. Fakat bunun dışındaki durumlarda bu yöntem işe yaramayacak veya pratik bir yöntem olmayacaktır.

Kablosuz ağlara çeşitli cihazlarla bağlanabilirsiniz. Bağlandığınız cihaz Windows veya Linux işletim sistemi kullanan bir PC, Mac OS kullanan bir Mac bilgisayar, veya akıllı telefon, tablet gibi bir mobil aygıt ise bu yazıdaki yöntemlerle daha önce bağlanılmış ağların şifresini bu cihazlar üzerinden görebilirsiniz. Bu ağ bilgileri bağlanıldığında cihaz tarafından kaydedilir ve özel bir dosya içerisinde saklanır. Ağ ismi ve şifre değiştiğinde cihaz artık ağa bağlanamaz. Bu yüzden cihazda "Bağlantıyı unut" seçeneğine tıkladığınızda bu veriler cihazınızdan silinir ve yeniden bağlanmaya hazır hale gelir.

**Windows**

Windows 10 tabanlı bir bilgisayarda ağ güvenlik anahtarını görüntülemek için ilk gerçekleştirmeniz gereken adım, ekranın sağ alt köşesindeki sistem bildirim alanında bulunan ağ simgesine sağ tıklayarak "Ağ ve Paylaşım Merkezi'ni Aç" seçeneğine tıklamanız olacak. Açılan pencerede sağ kolonda bulunan "Wi-Fi (Ağ ismi)" linkine tıklayacak, ardından yeni açılan pencerede "Kablosuz Özellikleri" butonuna tıklayacaksınız. Burada üstteki sekmelerden ikincisi olan Güvenlik sekmesine tıkladığınızda şifrenin bulunduğu sayfadasınız demektir. "Karakterleri göster" kutucuğunu işaretlediğinizde şifre görünür hale gelecektir.

İkinci yöntem olarak Başlat > Çalıştır kısmını açıp cmd yazarak Komut İstemi penceresini açtıktan sonra aşağıdaki komutu kendinize göre değiştirerek yazmanız olacak.

netsh wlan show profile name=ağ-adı key=clear

"ağ-adı" kısmına kendi Wireless ağınızın adını yazmayı unutmayın. Çıkan sonuçlar içinde "Security Settings" kısmının altında "Key Content"in karşısında ağ güvenlik anahtarı yazıyor olacak.

**Android**

Android işletim sisteminde bu gibi işlemler için root işlemi gerekir. Root işlemi gerçekleştirilmemişse ilgili klasörleri boş göreceksiniz. Telefon veya tabletin dosya yöneticisi üst klasörleri çıkmayı destekliyorsa cihaz klasörleri içerisinden "/data/misc/wifi" adresine gideceksiniz, desteklemiyorsa "Es File Explorer" uygulamasıyla deneyebilirsiniz. Bu klasör içerisinde "wpa\_supplicant.conf" isimli bir dosya yer alacaktır. Bunu herhangi bir metin editörüyle açın, Es File Explorer kullanıyorsanız uygulamanın kendi editörünü kullanabilirsiniz. Bu dosya içerisinde bağlandığınz tüm ağların güvenlik anahtarı görülecektir. SSID kısmının karşısında ağ adı, psk kısmında ise şifre yer alır.

**iOS**

iOS kullanan cihazlarda bu işlem için jailbreak gerekir. Daha sonra Cydia üzerindeki "Wifi Passwords" gibi uygulamalarla kayıtlı güvenlik anahtarlarını görebilirsiniz. Tabii telefonun güvenliği açısından bu tür işlemler için bu gibi uygulamalara pek güvenmemeniz gerekiyor.

**Mac OS**

Mac OS üzerinden CMD + Space tuşlarına basarak çıkan Spotlight arama kısmına "keychain" veya "anahtar" yazarak "Anahtar Zinciri Erişimi" (Keychain Access) sayfasını açacaksınız.  Ardından bu pencerede arama kutusuna wifi ağının ismini yazıp çıkan wifi ağ sonucunun üzerine sağ tıklayarak "Bilgi ver" (Get info) kısmını açacaksınız. Burada "Parolayı göster" (Show password) kutucuğunu işaretlediğinizde şifre karşınıa çıkacaktır.

İkinci yöntemde ise yine CMD + Space tuşları ile açtığınız Spotlight aramasına terminal yazacak ve ilgili pencereyi açtıktan sonra, aşağıdaki komutu "ağ-adı" kısmını kendi wifi ağınızın ismine göre düzenleyerek yazacaksınız.

security find-generic-password -wa ağ-adı

**Linux**

Ubuntu gibi bir dağıtım kullanıyorsanız ağ ayarları kısmından Wireless kısmına girerek diğer yöntemlerdekine benzer şekilde ağ şifresini görüntüleyebilirsiniz. Fakat Linux'un geneli için ve Linux mantığına da uygun olması açısından şimdi vereceğim yöntem daha idealdir. Linux dağıtımının terminal sayfasını açtıktan sonra aşağıdaki komutu "ağ-adı" kısmını kendi ağınızın ismi olacak şekilde düzenledikten sonra girin.

sudo cat /etc/NetworkManager/system-connections/ağ-adı | grep psk=

Ağ adını bilmiyorsanız aşağıdaki komutu kullanabilirsiniz.

sudo grep psk= /etc/NetworkManager/system-connections/\*

Çıkan sonuçların en altında "password" kısmının karşısında ağ güvenlik anahtarı yer alacaktır.
