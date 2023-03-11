# BANK
OOP PROJECT FOR BANK SYSTEMES
İçerik: Bir bankada çalışan kişilerin genel şemasını oluşturmak.
Amaç: GS Bank çalışanlarının yaptıkları işlere göre sınıflandırılması, bu kişilerin bilgilerinin kolay erişilebilir olması ve gerektiğinde bilgi değişiminin sağlanabilmesi amaçlanmıştır.

Kullanılan metotlar:
Çalışanların genel bilgilerine ulaşılabilecek ve daha sonrasında üzerinden miras alınabilecek ana sınıf olarak ‘’ Calisan” sınıfı oluşturulmuştur. Bu sınıfın içine bilgilerin atılması adına __init__ fonksiyonu tanımlanmıştır. Ayrıca tanımlı bilgilere ulaşılabilmek amacıyla da bir adet fonksiyon tanımlanmıştır. 
 
        
Sonraki adımda bir yönetici sınıfı “Yonetici” oluşturulmak istenmiştir. Bu sınıfı oluştururken  miras alma yönetimi kullanılmış, “Calisan” sınıfı içe aktarılmıştır.
 
Ancak girilen bilgilerde birtakım farklılıklar olması istendiği için __init__ fonksiyonu override edilmiştir.
 
Ayrıca bu sınıfın altında yöneticinin sorumluluğunda çalışan kişilerin bilgilerini eklemek, çıkartmak ve görebilmek için fonksiyonlar tanımlanmıştır.

“Ceo” sınıfı “Yonetici” sınıfında miras alınarak oluşturulmuştur.
 
Bu sınıfın içinde Ceo’nun bilgilerini gösterecek ve Ceo’nun sorumlu olduğu yöneticileri ekleyecek fonksiyonlar tanımlanmıştır.
Yazılımcılar için ayrıca bir sınıf açılmak istenmiştir. “Calisan” sınıfından miras alma yöntemi kullanılmıştır. Ayrıca __init__ fonksiyonu override edilmiştir.
 
Bu sınıfın altında da yazılımcıların kişisel bilgilerini ve bildikleri yazılım dillerini gösterebilen fonksiyonlar tanımlanmıştır.
Daha sonra sınıflara gerekli objeler oluşturulmuştur.
    

Daha sonra da sınıfların içindeki fonksiyonlar kullanılarak çalışanların yetkili kişilere ataması yapılmıştır.
  
 
 
Müşterileri ifade edebilmek amacıyla bir “musteri” sınıfı oluşturulmuştur. Bu sınıfın içine bilgilerin atılması adına __init__ fonksiyonu tanımlanmıştır ve bir adet mal varlığını ifade eden “malVarligi” fonksiyonu tanımlanmıştır.
 
 
Müşterilerle ilgilenen veznadarları belirtmek amacıyla “veznedar” sınıfı oluşturulmuştur. “__init__” fonksiyonunun yanısıra bu sınıfta kasada yapılan işlemleri tanımlamak üzere “kasayaParaGirdi” ve “kasadanParaCikti” fonksiyonları tanımlanmıştır.
 
Bu fonksiyonlar müşterinin bankaya nakit para yatırması veya çekmesi durumlarında: Müşterinin nakit parasındaki değişimi, (“müsteri.nakit”)                                              Müşterinin banka hesabındaki değişimi, (“müsteri.bankadakiParasi”)                          Bankanın kasasındaki para miktarının değişimini, (“kasasindakiPara”)                                          ifade edebilmek için kullanılmıştır.
Son sınıfımız olarak “ortak_hesap” sınıfı oluşturulmuştur. Bu sınıf hesaplarını birleştirmek isteyen müşterileri temsil etmektedir. Sınıfın altında __add__ fonksiyonu overloading metodu ile yeniden tanımlanmıştır. ”hesaptoplama” adıyla tanımlanan fonksiyonun amacı, hesaplarını birleştiren müşterilerin isimlerini bastırmak ve hesaplarındaki paraları birleştirmelerini sağlamaktır. 
Bu class seçilen müşterilin ortak hesaba geçmek istemesi takdirinde sahip oldukları parayı görmeye yarıyor.Gelişmiş aşamalarda buradan toplanılan paralar ve müşteri isimleri ile birlikte BirlikteHayatBirlikteHesap class'ı oluşturalacak ve kullanıcalar tek bir hesabı birlikte yönetebilecekler.
 
 
