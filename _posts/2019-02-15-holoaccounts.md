---
layout: post
title: Cüzdanlar, Borsa Hesapları ve Holo Hesapları
---

#### Geçtiğimiz haftalarda kimliğinizi kontrol etme , verilerinize sahip olma ve hesabınız için hem çekirdek hem de özel anahtar bulundurma konusunda konuşuyorduk. Ama bu ne anlama geliyor? Bu yazıda, cüzdanların, hesap alışverişlerinin ve HoloFuel hesaplarının çalışma şeklini daha da tanımlamayı ve her birinin uyguladığı güvenlik mekanizmalarını keşfetmeyi hedefliyoruz.


![_config.yml]({{ site.baseurl }}/images/holo.png)

**Early Crypto** meraklıları arasında ortak bir iddia vardı: “**Özel anahtarlara sahip değilseniz, bitcoinlere sahip değilsiniz.”** Bu anlayış, temel olarak ulusal para sistemlerinin ana eleştirilerinden birinin bir uzantısıdır; İnsanlar, bir bankada veya bankanın kendisi veya hatta devlet kurumları tarafından değiştirilebilecek açık ve erişilebilir bir hesapta saklanırsa, kontrolün gerçekten birinin kendi ulusal fiat parasına sahip olduğunu sorguluyorlar.

Hesaplarda ortaya çıkabilecek sorunlar, kripto'nun vahşi batısında daha da problemlidir. İlk güvenlik protokolleri ve bankacılık endüstrisinin tabi olduğu düzenleyici gözetim olmadan, borsalar ve bunların içindeki hesaplar birçok kesmenin hedefi olmuştur. Hackchain kripto para alım satım borsalarının bir listesi olan **Blockchain Mezarlığı (Blockchain Graveyard)** büyümeye devam ediyor. CipherTrace'nin endüstri raporunda bildirildiği gibi korsanların kripto para birimi borsalarından ve diğer platformlardan çalınan **927 milyon dolar**ın üzerinde olması, kripto para sahiplerinin çeşitli platformlarda barındırıldıklarında fonlarının güvenliği ve bütünlüğü konusunda endişeli olmaları için kesinlikle haklı.

*Ancak bu olayların biraz önüne geçiyor..* Haydi geri adım atalım ve kripto para birimleri için kullanılabilecek farklı depolama türlerini ve kullandıkları güvenlik türlerini anlamak için tanımlayıcı çalışmalar yapalım. Öncelikli hedefimiz cüzdanları borsa hesaplarından ayırt etmek ve Holo Hesabı kavramını tanıtmak, özellikle de HoloFuel Hesabı olmaktır.

# - Cüzdanlar (wallets)

İki temel cüzdan kategorisi vardır: **soğuk** olan; genellikle özel anahtarların tamamen çevrimdışı olduğu ve Internet bağlantısı olan cihazlarda çalışan sıcak olanları. Soğuk depo seçenekleri arasında kağıt cüzdanlar ve donanım cüzdanları; **sıcak** cüzdan seçenekleri arasında **mobil cüzdanlar, masaüstü cüzdanlar ve çevrimiçi (web) cüzdanlar bulunur.**

Kripto para oluşturma işleminin temel nedenlerinden biri, sahibinin kendi parasını koruyabilmesi ve bunu yapmak için başka bir güvenilir üçüncü tarafa bağımlı olması gerekmemesidir. Sıcak veya Soğuk cüzdan seçenekleri arasındaki seçenekler temel olarak hız ve verimliliği güvenlik endişeleriyle karşılaştırır.

Anahtarların tamamen çevrimdışı olduğu soğuk depolarda, güvenlik analistlerinin çoğuna göre sahip olabileceğiniz en iyi korumadır. Çevrimdışı bir cüzdan kullanmak, kendi paranızı korumanıza yardımcı olabilir - ancak özel anahtarlarınızı kaybederseniz, paranızı geri kazanmanın** hiçbir yolu olmadan otomatik olarak kaybedersiniz**. Şifrenizi sıfırlama seçeneği yoktur. **Kağıt cüzdanlar**, endüstrideki en ucuz soğuk cüzdan olarak belirlenmiştir. Madeni para veya tokenları halka açık bir adrese aktardığınızda, fonlar güvende olur. Kağıt cüzdanlar banknot gibi çalışır; çalınabilirler ve yangın veya sel durumunda fiziksel olarak tahrip olabilirler. Kağıt cüzdanlar, güvenli cihazlarda oluşturulmuşsa kötü amaçlı yazılım ve bilgisayar korsanları için ulaşılmaz olur ancak yeni başlayanlar için kafa karıştırıcı olabilir.

**Donanım cüzdanları** daha pahalıdır. Bunlar, Trezor veya Ledger Nano S gibi satın aldığınız fiziksel cihazlardır. Bu tür cihazlar, özel anahtarları çevrimdışı olarak depolar; bu nedenle, kötü amaçlı yazılım bulaşmış bir bilgisayara bağlı olsalar bile, nispeten güvenli oldukları anlamına gelir. Bir bilgisayar korsanının bir işlemi tehlikeye atma girişiminde, bilgisayar korsanı özel anahtarlara erişemeyeceğinden fonlar korsan tarafından kullanılamaz.

Soğuk cüzdanlar internetten ayrı tutulsa da, sıcak cüzdanlara bağlı seçeneklerdir ve genellikle harcamaları mümkün olduğunca elverişli hale getirerek ödemeleri almanın en kolay yolu olarak kabul edilir. Genel olarak, sıcak bir cüzdanda çok miktarda kripto para birimini bulundurmanız önerilmez. **Web cüzdanları **en düşük güvenlik seviyesini sunar; en güçlü avantajı, internete bağlı herhangi bir cihazdan erişilebilir olmalarıdır. Ayrıca mobil cüzdan gibi çevrimiçi cüzdanlarınızı da kaybedemezsiniz. Web cüzdanları, dolandırıcı ve bilgisayar korsanları için en kolay hedeflerdir ayrıca cüzdanı tamamen kontrol altında tutmanıza izin vermeyecek ancak cüzdanı etkin bir şekilde merkezi hesaba dönüştürecek sağlayıcılar da vardır. Bunlar tavsiye edilmez. **Masaüstü cüzdanlar** en yaygın kullanılan sıcak cüzdan türü olmaya devam ediyor - kullanımı kolay, nispeten güvenli, aralarından seçim yapabileceğiniz çeşitli seçenekler ve indirmek ücretsiz. Masaüstü cüzdanlarının çoğuna yalnızca yüklendikleri makineden erişilebilir.

# - Borsa Hesapları (exchange wallets)

Büyük olasılıkla çoğu kişi, özel anahtarları kontrol etmez ve istemez bu da Borsa hesabını cüzdandan ayıran şeydir.

Güvenlik açısından çoğu borsa, varlıklarının çoğunluğunu **(% 97 +)** soğuk depoda tutar. Bu anahtarların çevrimdışı olarak barındırıldığı ve fonların bilgisayar korsanları için erişilemez olduğu anlamına gelir.
Kripto para birimi değiş tokuşlarına gelince en savunmasız işlem, kullanıcılar hesaba kripto para birimlerini aktarırken kullanılan sıcak cüzdanlara yapılan bir saldırıdır.

Bir kripto para birimi borsa hesabında, borsanın kendisi ile ilgili olmayan fonların tutulması ile ilgili diğer riskler vardır. Bunlar arasında **güvenli olmayan bilgisayarlar, güvenli olmayan WIFI ağları, güvenilir olmayan eklentiler, orijinal web sitelerine benzer etki alanı olan dolandırcılar ve sahtekar web siteleri, zayıf şifreler, 2 faktörlü kimlik doğrulama eksikliği, kullanıcının e-postalarına veya telefon numaralarına yetkisiz erişim** ve **hesabın ihlali **sayılabilir. Bu istismarlar, esas olarak deneyimsiz kullanıcıları ve potansiyel olarak, kişisel cüzdanlarda fon sağlayan kullanıcıları hedeflemektedir. Riskler, ayrıca regulasyonlar ile de ilgili olabilir; eğer borsalar suç faaliyetinde bulunuyorsa, hükümetlerin fonları borsada dondurmaları mümkün. Kripto para birimi değişimi, bilgisayar korsanlarının ve DDOS saldırılarının hedefidir ya da bu değişim yetkililer tarafından durdulabilir ve fonlarınıza erişmek istediğiniz zaman kullanılamaz olduğu gözlemlenebilir. Temel olarak, bu risklerin büyük bir çoğunluğu, kriptonunuzun depolandığı cüzdanı kontrol etmediğiniz gerçeğinin temelini oluşturur.

# - Holo (Yakıt) Hesapları (holofuel accounts)

Cüzdanlar, Borsa Hesapları ve Holo (Yakıt) Hesapları arasında doğrudan bir karşılaştırma yapmak zordur çünkü kavramsal kategorilere baktığımızda aynı değildir.

Holochain dağıtılmış bir uygulama çerçevesidir. Holo, dağıtılmış bir barındırma platformudur. HoloFuel bir para birimi ve Holochain çerçevesinin üstünde çalışan ve Holo barındırma platformunun bir parçası olan bir uygulamadır. Önceki Holo AMA'da, Holochain'i veri bütünlüğü motoru olarak tanımladığımı duymuş olabilirsiniz. Bunun nedeni, Holochain'ın paylaşılan ve güvenli bir bağlam içinde çalışan dağıtılmış uygulamaları etkinleştirmek üzere tasarlanmasıdır.

HoloFuel ile aynı anda başka bir agent'in hesabını kredilendirmeden agent hesabınızı gönderemez veya borçlandırılamazsınız. Bu, çift girişli muhasebeye benzer bir etki yaratır; Her bir ajan zinciri hesap planındaki tek bir hesabın karşılığıdır. Bu muhasebe oyununun kuralları kodda tanımlanmıştır. Her iki katılımcı da ilk önce aynı kurallara göre oynadıklarından emin olduktan sonra bu işlem bu kuralları yerine getiriyor. Geliştirici belgelerimizi okuyorsanız, bu kurallar (kod) DNA olarak ifade edilir.

Şimdi, Holochain uygulamaları ve HoloFuel Hesabınız için güvenli bağlamda neyi kastettiğimizi özetleyelim.

-  **Karşılıklılık ve Rıza**: Kripto para birimleri tipik olarak spender'den gelen tek bir imzaya dayanarak çalışır. Alıcının işlem için taraf olduklarını bile bilmediğine dair bir kanıt yok, fonlar çalındığında kanıt bulma oranı düşük. HoloFuel ile işlemler karşılıklı olarak bilen ve rıza gösteren agentlar arasındadır ve bu rıza her agentin her iki zincire de kaydedilen işlem üzerindeki karşı imzalarıyla gösterilir.
- **Gerçekleştirilemezlik ve Doğrulanabilirlik**: İşlemler dağıtılmış karma tablo (DHT) ile nasıl etkileşimde bulundukları nedeniyle doğrulanabilir ve değişmezdir. Temsilciler ilk önce diğer tarafın durumunu (imza tarihini) inceler ve sözleşmelerini kriptografik olarak imzalarlar. Başlıklar daha sonra DHT'ye kaydedilir.
- **Anahtar Yönetimi**: Anahtarlarınız veya zinciriniz kaybolur yada çalınırsa, ana tohumunuzu önerildiği gibi yazdığınız sürece kullanımda olanları iptal edebilir ve hesabınızı kontrol altında tutarak başkalarının kullanmasını önlemek için yenilerini başlatabilirsiniz.
- **HoloFuel**'in geçerli işlemlerini yapabilmek için hem hesabın kaynak zincirini hem de özel anahtarların bulundurulması gerekir.

Bu tanıtımın **Holo ve HoloFuel** Hesapları hakkında bilgi isteyenler için yararlı olacağını umuyoruz. Gelecek hafta daha teknik bir yazı gelecek ve topluluğumuzun bazı teknik sorularına cevap vermek için AMA'da geliştiricilerimizden bir veya daha fazlasının yanımızda olmasını planlıyoruz. Her zaman olduğu gibi, girişinizi ve geri bildirimlerinizi **memnuniyetle** karşılıyoruz.

> Bu makale Mary Camacho'nun Wallets vs. Exchange Accounts vs. Holo(Fuel) Accounts adlı makalesinden ( https://medium.com/h-o-l-o/wallets-vs-exchange-accounts-vs-holo-fuel-accounts-60c10ff1b946 ) siz degerli Holochain Türkiye aile için Türkçe'ye çevrilmiştir.

Kusurumuz olduysa affola,
coinciyiz / -**f13end**
