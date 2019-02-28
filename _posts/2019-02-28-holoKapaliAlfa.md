---
layout: post
title: Holo Kapalı Alfa Testnet Tanıtımı
---

**Holo ağı,** Holochain'in yeni dağıtılmış uygulama ortamından internetin merkezi dünyasına bir köprüdür. Kapalı Alfa Testnetimizin piyasaya sürülmesiyle birlikte, İnternet tarayıcılarında erişilebilen dağıtılmış Holochain uygulamalarının uçtan uca bir testi için gerekli anahtar bileşenleri ve uygulamaları başlatıyoruz. Daha önce hiç yapılmamış ve teknolojideki yenilikleri kullanarak **gizlilik ve kontrol** alanındaki yenilikleri günlük internet kullanıcılari için kullanılabilir hale getiriyoruz. 

Holo'nun birçok entegre donanım, ağ, uygulama, servis ve protokol katmanından oluştuğunu açıkça belirtmenin önemli olduğunu düşünüyorum. Yalnızca Holo GitHub hesabında, 55 farklı depo vardır ve bunların yaklaşık 35 tanesi bu sürüm için aktif durumdadır - tüm Holochain kod depolarına ek olarak Holo'da **"aktif"** bir sürüme gecmek icin birçok hareketli parçanın bulunduğu karmaşık ve entegre bir işlem devam etmektedir. Kapalı Alfa Testnet yeni ve dağıtılmış bir internete olan yolculuğumuzda büyük bir başarı ve kilometre taşıdır. Şu anda sürüm için son birim test ve entegrasyon testlerini bitiriyoruz.

Bu kısa yazı ile yapmayı hedeflediğimiz şey, Kapalı Alfa Testnet için etkinleştirilen temel altyapı bileşenlerini ve uygulamalarını tanıtmak ve iç ve dış katılımcılarımız tarafından test edilecek olanı paylaşmaktir.

***" Hedefimiz gizlilik ve kontrol alanındaki yenilikleri İnternetin günlük kullanıcıları için kullanılabilir hale getirmektir ."***

## DeepKey 
Dağıtılmış Acik Anahtar Altyapısı (DPKI). DeepKey, Holo ve Holochain'deki anahtarları yönetmek için kullanılan bir araçtır. Holochain ile her uygulama için farklı bir anahtar çifti kullanilacaktir, bu da çok sayıda anahtar yönettiğiniz anlamına gelir. DeepKey, kullanıcıların Holochain Apps'ta kimliğin devamlılığını sağlar.

## Holo Ağ Altyapısı
Bu altyapı, dağıtılmış bir uygulamanın bir web kullanıcısının bir tarayıcı adres çubuğuna adresi yazmasına ve dağıtılmış uygulamayı son kullanıcıya ulaştırması için bir HoloHost'a yönlendirilmesine izin verir. Diğer ağ servisleri ise yüklü bir Holochain uygulaması kullanıcısının deneyimini simüle eden bir kullanıcının tarayıcı ve cihaz üzerinden kriptografik olarak onaylanmasını destekler.

## Holo Hosting İşletim Sistemi Sanal Makinesi
Kapalı Alfa için Holo Hosting OS Image çalıştıran bir sanal makine görüntüsünü kullanacaktır. Bu sanal makine görüntüsü önceden yüklenmiş Holochain ile birlikte gelir. Başlatma işlemi sırasında, Hosts için şifreleme anahtarları üretilecek ve cihaz Holo ağına kaydedilecektir.

## Holo Hosting Uygulaması
Holo Hosting İşletim Sisteminde önceden yüklenmiş olarak geliyor. Bu Uygulama, uygulama saglayicilarinin internet kullanıcıları için yayınlamak istedikleri uygulamaları belirlemelerine ve HoloHosts cihazlarında barındırmak istedikleri uygulamaları seçmelerine izin verir. Kullanıcı Arabirimi, barındırma etkinliklerini görüntülemek ve yönetmek için özel olarak bir uygulama sağlar.

## Holo Servis Günlüğü Uygulamasi
Ana bilgisayarın bant genişliğini ve işleme kullanımını izleyen uygulamadir. Bir Holo Hosting Cihazı, bir Holo web kullanıcısı adına işlev gördüğü için ilgili Holo Servis Günlüğü Uygulaması imzalı servis günlüklerini toplar. Bir HoloHost için yeterli servis günlüğü alındığında, bir “Servis Belgesi Faturası” oluşturulur ve ilgili Uygulama Sağlayıcısina gönderilir. Bu fatura ödeme yapilmasi için ön provizyondur.

## Holo hApp Mağazası
Uygulama Sağlayicilarinin uygulamaları yönettiği ve p2p kullanımı için başkalarının yüklemesi için uygun hale getirdiği yerdir. Kapalı Alfa Testnetinde bu yüklenebilir uygulamalara bağlantılar içeren bir web sitesi olarak uygulanacak ve herhangi bir hApp yükleme yetkisi Holo Ekibi ile sınırlı olacaktır.

## HoloFuel Uygulaması
HoloFuel Uygulamasi karşılıklı kredi para muhasebe için bir Holochain uygulamasıdır. Holo kullanıcılarının **'değer'** alışverişinde bulunmalarına izin verir ve Holo Uygulama Sağlayıcıları HoloHosts'un ucretini karsiladiginda Holo Hosting App tarafından kullanılır. Kapalı Alfa Testnet'imizde bu uygulama, **‘test HoloFuel’** kullanarak Uygulama Sağlayıcıları ve HoloHosts arasındaki ödemelerin yanı sıra, barındırma için faturalandırma işlemlerini de destekleyecektir.

## HoloPortlar
Üretim montajından, HoloPortlarin Kapalı Alfa Testnet sırasında iç ekip test uzmanlarına ulaşması bekleniyor. Holoport-OS Sanal Makinesi ile birlikte test edilecekler ve OS'nin en son sürümüne otomatik olarak güncelleme yapmalarını sağlayacaklar.

Yukarıdaki bileşenlerin tümü, Kapalı Alfa Test Ağımızın bir parçasıdır. Bu tür bir altyapı sürümündeki karmaşıklık seviyesi nedeniyle, bileşenleri üç dalga halinde aşamalı olarak test ediyoruz. Her bir dalgayla test ettiğimizi genişleteceğiz ve daha geniş bir test kitlesi davet edeceğiz.

**Kapalı Alfa Testneti için nihai hedeflerimiz:**

Teknik altyapisi olmayan kullanıcıların bilgisayarlarına Holo Hosting Cihazlarını yapılandırabilecekleri ve çalıştırabilecekleri bir Holo-Host Isletim Sistemi veya Sanal Makine Görüntüsü kurmalarını sağlamak ve Internet üzerinden Holochain dağıtılmış uygulamaları sunma yeteneğine sahip bir Holo test ağı sağlamak.

**Holo ve Yaklaşan Kilometre Taşları**

Bu Kapalı Alfa Testnet için bir araya gelen her şey için heyecanlıyız. Gelecek ay boyunca, Kapalı Alfanın test ve geri bildirimlerini izleyeceğiz ve bu sonuçlara dayanarak, aşağıda belirtilen gelecek Kilometre Taşlarıyla nasıl ilerleyeceği hakkındaki beklentilerimizi paylaşacağız.

HoloPortlarin topluluğumuzdaki birçok kişi için, özellikle de IGG destekçileri için önemli bir kilometre taşı olduğunu biliyoruz. HoloPortlar, dağıtım merkezlerine yerleştirilmeden önce son montajın adımlarını attığından ekibimizin çoğu HoloPort sahiplerinin harika bir deneyim sağladigindan emin olmak için nelerin gerekli olduğuna odaklanıyor. Yukarıda listelenen bileşenlerin kapsamlı bir şekilde test edilmesi HoloPortlarin yakında inandığımız vizyon ve değerle ilgili olarak alacağı yegane şeydir.

**Holo yaklaşan kilometre taşları şunlardır:**
- HoloPortlar, Distribütörlere ve Son Kullanıcılara sevk edilmesi
- Holo Açık Alfa Testnet
- Holo Tam Özellikli Testnet
- Holo Beta Main-net


> Bu yazi  https://medium.com/h-o-l-o/introducing-holo-closed-alpha-testnet-fc9d95efab21 adresinde siz degerli **Holochain Turkiye komunite uyeleri** icin Turkce'ye cevrilmistir.

**Bir kusurumuz olduysa affola;**
twitter.com/**coinciyiz**
**`f13end**


