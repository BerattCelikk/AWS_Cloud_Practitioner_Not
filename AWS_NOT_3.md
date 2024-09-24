# 🌐 AWS Temelleri

## Neden AWS Tercih Etmelisiniz? 
AWS, kullanıcıların yalnızca kullandıkları kadar ödeme yapmalarını sağlayan esnek bir model sunar. Örneğin, **Amazon EC2** ile gereksinimlerinize uygun sayıda sanal sunucu başlatabilir, kaynakları ihtiyacınıza göre dinamik bir şekilde yönetebilirsiniz.

---

## Bulut Bilişim Nedir? 
**Bulut bilişim**, bilgi teknolojisi kaynaklarının internet üzerinden talep üzerine sunulmasıdır. Bu model, kullanıcıların sadece kullandıkları hizmetler için ödeme yapmalarını sağlar. Altyapı, platform ve yazılım gibi farklı katmanlarda hizmetler sunarak iş süreçlerini kolaylaştırır.

---

## AWS, Pay-As-You-Go Modelini Nasıl Sunuyor? 
AWS, çeşitli sanal makineleri (instance) aynı fiziksel donanım üzerinde izole ederek kaynakları verimli bir şekilde kullanır. Örneğin, benim şirketim ve John'un şirketi, AWS’ye ait aynı sunucuyu paylaşabilir; ancak sanal makinelerimiz tamamen bağımsızdır. Bu yöntem, kullanıcıların kendi veri merkezlerini yönetme maliyetlerini azaltır ve daha düşük maliyetli hizmet sunar.

---

## AWS EC2 Tanıtımı 

### EC2 ile Hangi İşletim Sistemlerini Kullanabilirsiniz? 
- 🖥️ **Windows:** Kullanıcı dostu arayüzü ve geniş uygulama desteği ile.
- 🐧 **Linux:** Açık kaynak yapısı sayesinde esneklik ve özelleştirme imkânı sunar.

### EC2 Üzerinde Hangi Yazılımları Çalıştırabilirsiniz? 
Neredeyse her tür yazılımı çalıştırabilirsiniz: web uygulamaları, veritabanları, özel yazılımlar, analiz araçları ve daha fazlası.

### EC2 Instance Türleri Nelerdir? 
Farklı görevler için özel olarak tasarlanmış EC2 instance'ları mevcuttur. Her bir tür, büyük bir organizasyondaki çalışanları departmanlar halinde gruplandırmak gibi, instance aileleri altında kategorize edilir.

### EC2 Instance Aileleri:
- **🔧 Genel Amaç (General Purpose):** Çeşitli iş yükleri, web sunucuları veya kod depoları için idealdir. **T2/T3** serileri örnek verilebilir.
- **⚙️ Hesaplama Optimizasyonu (Compute Optimized):** Oyun sunucuları, bilimsel simülasyonlar gibi hesaplama yoğun görevler için uygundur. **C5** serisi bu kategoride yer alır.
- **🧠 Bellek Optimizasyonu (Memory Optimized):** Bellek tüketimi yüksek olan uygulamalar için. **R5** serisi örnek verilebilir.
- **⚡ Hızlandırılmış Hesaplama (Accelerated Computing):** Kayan nokta hesaplamaları, grafik işleme ve veri akışı için idealdir. **P3** ve **G4** serileri bu türdeki uygulamalar için tasarlanmıştır.
- **💾 Depolama Optimizasyonu (Storage Optimized):** Yerel depolama alanında yüksek performans sunar. **I3** serisi, yoğun veri işleme için uygundur.

### EC2 Satın Alma Seçenekleri Nelerdir?
- **📅 Talep Üzerine (On-Demand):** Kullanıcılar, saatlik veya saniyelik bazda ödeme yapabilir. Bu seçenek, esneklik ve hızlı başlangıç için idealdir.
- **💰 Tasarruf Planları (Savings Plans):** 1 veya 3 yıllık taahhütle daha düşük fiyatlar sunar. Uzun vadeli projeler için büyük tasarruf sağlar.
- **🔒 Rezerve Edilmiş Instance'lar (Reserved Instances):** Sabit bir kullanım süresi olan projeler için uygundur; kaynak gereksinimleri tahmin edilebiliyor.
- **📉 Spot Instance'lar:** Talep üzerine fiyattan %90'a kadar indirim sağlayabilir. Ancak, AWS, bu instance'ları istediği zaman durdurabilir; bu nedenle kesintiye dayanıklı işler için uygundur.
- **🏢 Dedicated Host:** Tamamen özel bir sunucu olup, uyumluluk gereksinimleri olan kullanıcılar için idealdir. Diğer kullanıcılarla paylaşılmadığı için yüksek güvenlik sunar.

### Elastic Load Balancing (ELB) Nedir? 
Birden fazla EC2 instance'ınız varsa, **Elastic Load Balancer**, gelen uygulama trafiğini otomatik olarak kaynaklar arasında dağıtarak her bir instance’a iş yükünü dengeli bir şekilde yönlendirir. Bu, yüksek kullanılabilirlik ve ölçeklenebilirlik sağlar.

### Sıkı Bağlı Mimari Neden Sorunludur, Gevşek Bağlı Mimari Neden Avantajlıdır? 
Sıkı bağlı mimarilerde, bir uygulamadaki hatalar diğer bağlı uygulamalarda da sorunlara yol açabilir. Gevşek bağlı mimariler ise, uygulamalar arasında bağımsız bir çalışma ortamı sunar; böylece bir uygulama arızalandığında diğerleri etkilenmez.

### Gevşek Bağlı Mimari Nasıl Oluşturulur? 
Uygulamalar arasında bir **mesaj kuyruğu** oluşturarak bir tampon işlevi görebilirsiniz. Bu, uygulamaların birbirinden bağımsız bir şekilde çalışmasını sağlar ve sistem genelindeki dayanıklılığı artırır.

### AWS’nin Mesaj Kuyruğu Olarak Hangi 2 Servisi Bulunur? 
- 📬 **AWS SQS (Simple Queue Service):** Mesajları kuyrukta saklayarak gönderebilir ve alabilirsiniz.
- 📢 **AWS SNS (Simple Notification Service):** Abonelere (telefon numaraları, e-posta adresleri, web sunucuları) bildirim ve mesaj gönderebilir.

### AWS SQS Ne İşlevi Görür? 
SQS, her ölçekte mesaj gönderebilir, depolayabilir ve alabilir. Mesajları sıraya alarak sistemdeki yükü dengelemeye yardımcı olur.

### Payload Nedir? 
**Payload**, bir mesajın içerdiği veriler olup, genellikle uygulamalar arası iletişimde taşınan asıl verilerdir.

### AWS SNS Ne İşlev Görür? 
SNS, abonelere (telefon numaraları, e-posta adresleri, web sunucuları, AWS Lambda Fonksiyonları) bildirim ve mesaj gönderir. Çoklu abonelere anında bilgi ulaştırarak sistemin etkinliğini artırır.

### AWS Lambda Nedir? 
**AWS Lambda**, bir olay tetiklendiğinde belirli bir işlevi veya script'i çalıştıran sunucusuz (serverless) bir bilişim platformudur. Bu platform, 15 dakikadan kısa sürede çalışacak kodları yönetirken, arka planda ölçeklenebilirliği de otomatik olarak sağlar.

### Alt Yapıya Erişim Gerektiğinde Hangi Araçlar Kullanılmalı? 
Eğer alt yapıya erişim gerektiriyorsanız, AWS **Elastic Container Service (ECS)** veya **Elastic Kubernetes Service (EKS)** gibi bir konteyner orkestrasyon aracı kullanmalısınız.

### Konteyner Nedir? 
Konteyner, uygulamanızı paketleyen ve uygulamanın çalışması için gereken tüm bileşenleri içeren bir yapıdır. Docker konteynerleri, EC2 instance'ında çalıştırılır.

---

## AWS Küresel Altyapısı

### Erişilebilirlik Bölgesi (Availability Zone) Nedir ve Neden Uygulamanızı Birden Fazla Erişilebilirlik Bölgesinde Yaymalısınız? 
Erişilebilirlik bölgesi, AWS veri merkezlerinin bir grup lokasyonudur. Bu bölgeler, coğrafi olarak farklı alanlarda yer alır, böylece bir felaket durumunda hepsinin birden çökmesi önlenir; aynı zamanda düşük gecikme süresi sağlar. Uygulamanızı en az iki erişilebilirlik bölgesinde çalıştırmak, bir bölge sorun yaşadığında diğerinin aktif kalmasını garanti eder.

### Edge Location Nedir? 
**Edge location**, Amazon CloudFront'un içeriklerinizi müşterilere daha yakın bir konumda önbelleğe aldığı alanlardır. Bu, verinizin daha hızlı ulaşmasını sağlayarak kullanıcı deneyimini geliştirir.

---

## AWS ile Nasıl Çalışılır? 
AWS kaynaklarıyla **Yönetim Konsolu**, **Komut Satırı Arayüzü (CLI)**, **Yazılım Geliştirme Kitleri (SDK)** veya diğer araçlar aracılığıyla çalışabilirsiniz. Yönetim Konsolu, web tarayıcınız üzerinden erişilebilir.

- **CLI**, otomatikleştirilmiş görevler için güçlü bir araçtır. Çok sayıda instance oluşturmak veya yönetmek için idealdir.
- **SDK'lar**, belirli programlama dilleri aracılığıyla AWS’ye erişim sağlar; bu sayede uygulama geliştiriciler, AWS kaynaklarını kod ile yönetebilir.

### AWS Elastic Beanstalk Nedir? 
**AWS Elastic Beanstalk**, geliştiricilere uygulama dağıtımını ve yönetimini kolaylaştıran bir platformdur. AWS EC2 tabanlı ortamları hızlıca oluşturmanıza yardımcı olur ve otomatik ölçekleme, yük dengeleme gibi özellikler sunar.

### AWS CloudFormation Nedir? 
**AWS CloudFormation**, birçok AWS kaynağını "infrastructure as code" (kod olarak altyapı) yöntemiyle kontrol etmenizi sağlayan bir araçtır. **CloudFormation Templates** formatında JSON veya YAML dosyaları oluşturarak altyapınızı otomatikleştirebilirsiniz.


# 🚀 Veritabanı Performansınızı Hızlandırmanın Yolları

Veritabanı performansınızı artırmanın birkaç yolu bulunmaktadır:

- **⚡ Önbellek Katmanları Eklemek:** Veritabanınıza önbellek katmanları ekleyerek okuma sürelerini milisaniyelerden mikro saniyelere düşürebilirsiniz. **Amazon ElastiCache**, bu önbellek katmanlarını sağlamak için kullanılabilir.

- **🛠️ DynamoDB Accelerator (DAX):** Eğer **DynamoDB** kullanıyorsanız, DAX’ı kullanarak verilerinizin okuma sürelerini önemli ölçüde iyileştirebilirsiniz.

---

# 🔒 AWS Güvenlik Hizmetleri ve Modelleri

## AWS Paylaşımlı Sorumluluk Modeli
**AWS**, bulutun güvenliğinden sorumlu iken, kullanıcı bulut içindeki güvenlikten sorumludur. Bu model, her iki tarafın sorumluluklarını net bir şekilde tanımlar.

---

## AWS ve Kullanıcının Sorumlulukları
- **AWS:** Donanım, ağ ve sanal makineleri oluşturan hypervisor yazılımının güvenliğinden sorumludur.
  
- **Kullanıcı:** İşletim sistemi, uygulama ve veri güvenliğinden sorumludur.

---

## AWS Hesap Root Kullanıcısı Nedir?
**Root kullanıcı**, hesapta bulunan tüm kaynaklara erişim ve kontrol sağlar. **MFA (çok faktörlü kimlik doğrulama)** uygulamak son derece önemlidir.

---

## AWS IAM Nedir?
**AWS Identity and Access Management (IAM)**, kaynaklara erişimi yönetmek ve kontrol etmek için kullanılan bir sistemdir. IAM kullanıcıları oluşturabilir ve varsayılan olarak bu kullanıcıların hiçbir izni yoktur.

- **🔑 En Az Ayrıcalık İlkesi:** Kullanıcılar, yalnızca ihtiyaç duydukları erişim iznine sahip olmalıdır.

---

## IAM Grupları Nedir?
**IAM grupları**, aynı izinlere sahip kullanıcıların oluşturduğu gruplardır. Bu izinler, politikalar aracılığıyla uygulanır.

---

## IAM'deki Roller Nedir?
**Roller**, belirli eylemleri onaylayan veya reddeden ilişkilendirilmiş izinler içerir. Bu roller, geçici süreliğine kullanılabilir ve kullanıcılara geçici izinler sağlar.

---

## AWS Organizasyonları Nedir?
**AWS Organizasyonları**, birden fazla AWS hesabını yönetmek için merkezi bir yerdir. Ayrıca, tüm hesaplar için faturalamayı konsolide edebilir ve hiyerarşik hesap grupları oluşturabilirsiniz. Her hesap için erişebileceği AWS hizmetleri ve API'leri kontrol edebilirsiniz.

- **🔐 Servis Kontrol Politikaları (SCP'ler):** Organizasyondaki hesaplar için maksimum izinleri belirlemek üzere kullanılır. SCP'ler, Organizasyon Birimleri (OU'lar) veya bireysel hesaplar üzerine uygulanabilir.

---

## AWS Artifact Nedir?
**AWS Artifact**, AWS'nin uyumlu olduğunu kanıtlayan belgeleri talep edebileceğiniz bir platformdur. Ayrıca, HIPAA gibi belirli uyum yasaları için AWS Artifact Anlaşması imzalayabilirsiniz. AWS güvenlik kontrollerinin kanıtlarına da erişebilirsiniz.

---

## Müşteri Uyum Merkezi Nedir?
**Müşteri Uyum Merkezi**, uyum hakkında daha fazla bilgi edinmenize yardımcı olacak kaynakları içerir.

---

## DDoS Nedir?
**DDoS** (Dağıtık Hizmet Reddi), altyapınıza yönelik bir saldırıdır. Sistemlerinizi aşırı yüklemeye çalışarak çalışamaz hale getirmeyi amaçlar.

---

## Slowloris Saldırısı Nedir?
**Slowloris**, DDoS saldırı türlerinden biridir. Kötü niyetli istemci, sunucuya paket göndermeyi çok uzun bir süre alarak yapar. Bu, bir kafede sipariş vermeye çalışan birinin yavaş davranmasının, diğerlerinin beklemesini sağlaması gibi düşünülebilir. Slowloris isteğini tamamlamadığından, sunucu açık kalır ve mevcut bağlantı havuzunu doldurur, böylece diğer istemcilerin hizmet almasını engeller.

---

## AWS Mimarisi DDoS Saldırılarını Nasıl Önler?
**Güvenlik grupları**, yalnızca belirlediğiniz trafiğe izin verir. Güvenlik grupları, AWS ağ seviyesinde çalışır (EC2 örnek seviyesinde değil). Onayladığınız trafik dışındaki tüm trafiği engeller.

---

## AWS Shield ve AWS WAF Nedir?
- **🛡️ AWS WAF:** Web uygulama güvenlik duvarı kullanarak gelen trafiği kötü aktörlerin imzalarıyla filtreler. Makine öğrenimi yetenekleri ile tehditleri zamanla algılayabilir.
  
- **🛡️ AWS Shield:** DDoS koruması sağlar. Gelişmiş sürümü kullanılmadığı sürece ücretsizdir.

---

## Şifreleme Nedir?
**Şifreleme**, verilerinizi yalnızca yetkili tarafların erişebileceği bir şekilde güvence altına alır.

---

## AWS KMS Nedir?
**AWS Key Management Service**, şifreleme anahtarlarınızı yönetir.

---

## Amazon Inspector Nedir?
**Amazon Inspector**, uygulamalarınızın güvenliğini ve uyumunu artırmak için altyapınıza karşı otomatik bir güvenlik değerlendirmesi yapar. Güvenlik açıklarınızı ortaya çıkarır.

- **🔍 Üç Bileşenden Oluşur:**
  - Ağ yapılandırma erişilebilirliği,
  - Amazon ajanı,
  - Güvenlik değerlendirme hizmeti.

---

## Amazon GuardDuty Nedir?
**Amazon GuardDuty**, verilerinizi analiz ederek tehditleri tanımlar. Bağımsız olarak çalışır ve iş yüklerinizin performansını etkilemez.

# 📊 AWS İzleme ve Analitik Hizmetleri

## İzleme Nedir?
**İzleme**, sistemlerin gözlemlenmesi, metriklerin toplanması ve bu verilerin karar vermek için kullanılması anlamına gelir.

---

## Amazon CloudWatch Nedir?
**Amazon CloudWatch**, AWS altyapınızı ve uygulamalarınızı gerçek zamanlı olarak izlemenizi sağlar. 

- **⏰ Alarm Oluşturma:** CloudWatch, bir olay veya metrik tetiklendiğinde sizi bilgilendiren alarmlar oluşturmanıza olanak tanır. 
- **🔗 SNS Entegrasyonu:** Ayrıca, AWS SNS ile bağlantı kurarak bir kullanıcıya mesaj göndererek onları uyarmak mümkündür.
- **📊 Gösterge Tablosu:** Tüm verilerinizi tek bir yerde göstermek için CloudWatch gösterge tabloları oluşturabilirsiniz.

---

## AWS CloudTrail Nedir?
**AWS CloudTrail**, bir API denetim aracıdır. AWS'ye yapılan her isteğin kaydı, CloudTrail motorunda tutulur. Bu kayıtlar şunları içerir:

- İsteği kimin yaptığı
- İsteğin yapıldığı zaman
- İstemcinin IP adresi
- İsteğin yanıtı (reddedildi mi yoksa onaylandı mı)

- **🔍 CloudTrail Insights:** Ayrıca, hesabınızdaki olağan dışı API aktivitelerini tespit etmek için CloudTrail Insights’ı etkinleştirebilirsiniz.

---

## AWS Trusted Advisor Nedir?
**AWS Trusted Advisor**, kaynaklarınızı şu 5 temel ilkeye göre değerlendiren otomatik bir danışmandır:

- **💰 Maliyet Optimizasyonu**
- **⚡ Performans**
- **🔒 Güvenlik**
- **🛡️ Hata Toleransı**
- **📊 Hizmet Sınırları**

---

# 💰 AWS Fiyatlandırma ve Destek

## AWS Ücretsiz Katman
**AWS Ücretsiz Katman**, AWS’yi denemeniz için 3 farklı yol sunar:

- **🎉 Her Zaman Ücretsiz:** (sadece bazı hizmetler için)
- **🕒 12 Aylık Ücretsiz:** 
- **⏳ Deneme Süreleri:** (kısa süreli ücretsiz denemeler)

### Örnekler:
- **AWS Lambda:** Aylık 1 milyon ücretsiz istek (ve toplamda 3.2 milyon saniye işlem süresi… bu da 888 saattir).
- **AWS S3:** 12 ay boyunca 5 GB'a kadar depolama ücretsizdir.
- **AWS Lightsail:** 750 saate kadar bir ay deneme süresi sunar.

Daha fazla örnek arasında **AWS SageMaker**, **DynamoDB** (aylık 25 GB ücretsiz depolama), **SNS** ve daha fazlası bulunmaktadır.

---

## AWS Destek Planları
AWS, 4 farklı destek planı sunar:

1. **Temel Plan**
2. **Geliştirici Plan:** (destek için e-posta erişimi)
3. **İş Planı:** (destek için telefon erişimi)
4. **Kurumsal Plan:** (kritik iş yükleri için 15 dakikalık yanıt süresi ve özel Teknik Hesap Yöneticisi (TAM))

---

## İyi Mimarili Çerçevesinin 5 Temel İlkesi
AWS'nin İyi Mimarili Çerçevesi, aşağıdaki 5 temel ilkeye dayanır:

- **📈 Operasyonel Mükemmellik**
- **🔐 Güvenlik**
- **✅ Güvenilirlik**
- **⚙️ Performans Verimliliği**
- **💵 Maliyet Optimizasyonu**

Bir TAM, hesabınızı gözden geçirerek iyi mimari çerçevesine dayalı önerilerde bulunabilir.

---

## AWS Marketplace Nedir?
**AWS Marketplace**, AWS üzerinde çalışabilen binlerce bağımsız satıcının yazılımlarını içeren bir katalogdur.

---

# 🚀 AWS Göç ve İnovasyon

## AWS CAF Nedir?
**AWS Cloud Adoption Framework (CAF)**, kullanıcıların yerel verilerini (veya bulut verilerini) AWS’ye geçirmelerine yardımcı olan bir çerçevedir.

### CAF'nın 6 Perspektifi:
1. **📊 İş**
2. **👥 İnsanlar**
3. **🏢 Yönetim**
4. **🖥️ Platform**
5. **🔒 Güvenlik**
6. **⚙️ Operasyonlar**

---

## Göçün 6 R’si Nedir?
Mevcut ortamınızda tam olarak neler olduğunu öğrendikten sonra, göçünüz için en uygun olan 6 R’yi belirleyebilirsiniz:

- **🚀 Rehosting (Lift and Shift):** Uygulamanızı/altyapınızı sadece kaldırıp AWS’ye taşıma.
- **🔧 Replatforming (Lift, Tinker, and Shift):** Bulut optimizasyonları yapmadan önce bazı iyileştirmeler yapmak.
- **🗑️ Retire:** Altyapınızın bazı bölümlerinin artık gerekli olmaması.
- **🏗️ Retain:** Bazı altyapı bileşenlerinin yerel olarak kalması ancak AWS’ye taşınmaması (ve zamanla emekliye ayrılabilir).
- **🆕 Repurchase:** Eski yazılımları terk edip bulutta yeni bir şeye geçmek.
- **🔄 Refactoring:** Yeni kod yazmanız, yeni özellikler eklemeniz ve AWS’ye taşındıktan sonra her şeyin çalışmasını sağlamak için kodun mimarisini değiştirmeniz gerekecek.

---

## AWS Snow Ailesi Nedir?
**AWS Snow Ailesi**, verilerin fiziksel olarak AWS’ye taşınmasına yardımcı olan bir dizi fiziksel cihazdır. Örneğin, Amazon size AWS Snowcone gönderir; bu cihazı veri sunucunuza veya bilgisayarınıza takar, istediğiniz verileri kopyalar ve ardından geri gönderirsiniz. Verileriniz, örnek olarak bir S3 kovasına kopyalanmış olarak bulabilirsiniz.

### AWS Snow Ailesi Aletleri:
- **🌟 AWS Snowcone:** En küçük olanıdır ve 8 TB'a kadar depolama kapasitesine sahiptir.
- **📦 AWS Snowball:** Bir sonraki büyüklükteki cihazdır ve 2 versiyonu bulunmaktadır: 
  - **🔒 Depolama Optimize Edilmiş:** 80 TB
  - **⚡ Hesaplama Optimize Edilmiş:** 42 TB
- **🚛 AWS Snowmobile:** En büyük olanıdır ve kamyonla teslim edilir, 100 Petabayt (100,000 TB) kapasiteli veri taşıyabilir.

---

# 🌐 AWS Bulut Özeti

## AWS Well-Architected Framework Nedir?
**AWS Well-Architected Framework**, bulut mimarinizin en iyi uygulamalara uygun olup olmadığını değerlendiren bir çerçevedir. Şu beş temel ilkeyi içerir:

1. **🏆 Operasyonel Mükemmellik:** Mimarinin iş değerini sağlama ve sürekli iyileştirme.
2. **🔒 Güvenlik:** Verilerinizi ve sistemlerinizi şifreleme ile koruma.
3. **✅ Güvenilirlik:** Altyapı veya AWS'deki kesintilerden kurtulma planlamasına odaklanma, ayrıca yatay ölçeklenebilirlik.
4. **⚡ Performans Verimliliği:** Verimlilik için doğru hizmetleri ve hizmet türlerini seçme.
5. **💰 Maliyet Optimizasyonu:** Maliyetleri optimize etme.
6. **🌱 Sürdürülebilirlik:** Enerji tüketimini azaltarak kullanılan kaynaklardan maksimum fayda sağlama.

---

## AWS Well-Architected Tool Nedir?
**Well-Architected Tool**, mimarinizin AWS Well-Architected Framework standartlarına uygunluğunu kontrol eden bir araçtır. Bu araç, iyileştirme alanlarını da belirtebilir.

---

## AWS Kullanmanın 6 Ana Faydası
1. **💵 Sabit giderleri değişken giderlerle değiştirin:** Kullanıma göre ödeme modeli (pay-as-you-go).
2. **📈 Büyük ölçek ekonomilerinden yararlanın.**
3. **❌ Kapacity tahminine son verin.**
4. **⚡ Hız ve çevikliği artırın.**
5. **🏢 Veri merkezleri işletmeye para harcamayı bırakın.**
6. **🌍 Dakikalar içinde globalleşin.**

---

# 📚 Ek Notlar

## Paylaşılan Kontroller Nedir?
**Paylaşılan kontroller**, hem AWS'nin hem de kullanıcının sorumluluğu altında olan kontrollerdir. Bu kontroller şunları içerir:

- **🔄 Yamanın Yönetimi**
- **⚙️ Konfigürasyon Yönetimi**
- **📚 Farkındalık ve Eğitim**

---

## S3 Hakkında Not
**S3**, manuel olarak ölçeklendirilemez; bunun yerine otomatik olarak ölçeklenir. Herhangi bir tür veriyi saklayabilen sınırsız depolama sunar, ancak her bir nesnenin maksimum boyutu 5 TB'dır. Yani, **"sonsuz ölçeklenebilir"** bir yapıya sahiptir.

---

## Amazon ElastiCache Neden Kullanılır?
**ElastiCache**, bulutta bir bellek içi veri deposu veya önbellek dağıtımını ve yönetimini kolaylaştıran bir web hizmetidir. Hızlı veri erişimi gerektiren uygulamalar için idealdir; çünkü bir veritabanını sorgulamak her zaman önbellekten veri almak kadar hızlı değildir.

---

## 3 AWS Bulut Bilişim Modeli Nedir?
**AWS Bulut Bilişim Modelleri** şunlardır:

1. **🖥️ Altyapı Hizmeti (IaaS)**
2. **🛠️ Platform Hizmeti (PaaS)**
3. **📦 Yazılım Hizmeti (SaaS)**

Not: Ağ yönetimi, Altyapı Hizmeti'nin bir parçasıdır.

---

## AWS-Yönetilen Hizmet Nedir?
**AWS-yönetilen hizmet**, AWS'nin bu hizmetlerin işletim ve bakım yükümlülüklerini üstlendiği hizmetlerdir. 

Örnekler arasında **DynamoDB, Lambda, Elastic MapReduce, S3** gibi hizmetler yer alır. IAM, VPC ve EC2 bu hizmetlere dahil değildir; çünkü bunların yönetimi kullanıcıya aittir.

---

## Altyapı Olay Yönetimi Nedir?
**Altyapı Olay Yönetimi**, AWS Destek'ten alabileceğiniz kısa süreli bir hizmettir (Enterprise Destek planında dahil ve Business Destek planında satın alınabilir). Bu hizmet, büyük trafik olayları (ürün lansmanları ve reklam kampanyaları gibi) için mimari rehberlik sağlamada yardımcı olur.
