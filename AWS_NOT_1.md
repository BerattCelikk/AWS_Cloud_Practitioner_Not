# Bulut Bilişim

- [Bulut Bilişim](#bulut-bilisim)
  - [Bulut Bilişim Nedir?](#bulut-bilisim-nedir)
    - [Bulutun Dağıtım Modelleri](#bulutun-dagitim-modelleri)
    - [Bulut Bilişimin Beş Özelliği](#bulut-bilisimin-bes-ozelligi)
    - [Bulut Bilişimin Altı Avantajı](#bulut-bilisimin-alti-avantaji)
    - [Bulutun Çözdüğü Problemler](#bulutun-cozdugu-problemler)
    - [Bulut Bilişim Türleri](#bulut-bilisim-turleri)
    - [Bulut Bilişim Türlerine Örnekler](#bulut-bilisim-turlerine-ornekler)
    - [Bulutun Fiyatlandırması - Hızlı Bakış](#bulutun-fiyatlandirmasi---hizli-bakis)
    - [AWS Bulut Kullanım Alanları](#aws-bulut-kullanim-alanlari)
  - [AWS Küresel Altyapısı](#aws-kuresel-altyapisi)
    - [AWS Bölgeleri](#aws-bolgeleri)
    - [AWS Bölgesi Nasıl Seçilir?](#aws-bolgesi-nasil-secilir)
    - [AWS Erişilebilirlik Bölgeleri](#aws-erisilebilirlik-bolgeleri)
    - [AWS Uç Noktaları (Edge Locations)](#aws-uc-noktalari-edge-locations)
  - [AWS Konsolu Turu](#aws-konsolu-turu)
  - [Paylaşımlı Sorumluluk Modeli](#paylasimli-sorumluluk-modeli)
## Bulut Bilişim Nedir?

- Bulut bilişim, isteğe bağlı olarak işlem gücü, veritabanı depolama, uygulamalar ve diğer BT kaynaklarının teslim edilmesidir.
- Bir bulut hizmet platformu üzerinden kullanım başına ödeme modeli ile sunulur.
- Tam olarak ihtiyacınız olan türde ve boyutta bilgi işlem kaynaklarını tahsis edebilirsiniz.
- Neredeyse anında ihtiyaç duyduğunuz kadar kaynağa erişebilirsiniz.
- Sunuculara, depolama alanlarına, veritabanlarına ve bir dizi uygulama hizmetine basit bir şekilde erişim sağlar.
- Amazon Web Services, bu uygulama hizmetleri için gerekli olan ağ bağlantılı donanımı sağlar, siz ise bu kaynakları bir web uygulaması üzerinden kullanırsınız.
### Bulutun Dağıtım Modelleri

| **Özel Bulut (Private Cloud):**                                        | **Genel Bulut (Public Cloud):**                                                                       | **Hibrit Bulut (Hybrid Cloud):**                                              |
| --------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| Bir kuruluş tarafından kullanılan bulut hizmetleri, halka açık değildir. | İnternet üzerinden üçüncü taraf bir bulut sağlayıcısına ait bulut kaynakları.                          | Bazı sunucuları yerinde tutup bazı yetenekleri buluta genişletebilirsiniz.  |
| Tam kontrol                                                           | Bulut Bilişimin Altı Avantajı                                                                          | Özel altyapınızda hassas varlıklar üzerinde kontrol.                        |
| Hassas uygulamalar için güvenlik                                       |                                                                                                       | Genel bulutun esnekliği ve maliyet etkinliği.                               |
| Belirli iş ihtiyaçlarını karşılar                                      |                                                                                                       |                                                                            |
### Bulut Bilişimin Beş Özelliği

- **İsteğe Bağlı Self Servis:**
  - Kullanıcılar, servis sağlayıcı ile etkileşime girmeden kaynakları tahsis edebilir ve kullanabilirler.
- **Geniş Ağ Erişimi:**
  - Kaynaklar ağa bağlıdır ve çeşitli istemci platformlarından erişilebilir.
- **Çoklu Müşteri ve Kaynak Havuzlama:**
  - Birden fazla müşteri aynı altyapıyı ve uygulamaları güvenli ve gizli bir şekilde paylaşabilir.
  - Aynı fiziksel kaynaklardan birden fazla müşteri yararlanabilir.
- **Hızlı Esneklik ve Ölçeklenebilirlik:**
  - Gerektiğinde kaynakları hızlı bir şekilde edinir ve bırakır.
  - Talebe bağlı olarak hızla ve kolayca ölçeklenir.
- **Ölçülen Hizmet:**
  - Kullanım ölçülür, kullanıcılar ne kullandıysa ona göre ödeme yaparlar.
### Bulut Bilişimin Altı Avantajı

- **Sermaye Giderlerini (CAPEX) İşletme Giderlerine (OPEX) Çevirme**
  - Kullanım başına ödeme: Donanım sahibi olmaya gerek yok.
  - Toplam Mülkiyet Maliyeti (TCO) ve İşletme Giderleri (OPEX) azalır.
- **Büyük Ölçekli Ekonomilerden Faydalanma**
  - AWS, büyük ölçek nedeniyle daha verimli olduğu için fiyatlar azalır.
- **Kapasite Tahmini Yapmayı Bırakma**
  - Gerçek kullanım verilerine göre ölçeklendirin.
- **Hız ve Çevikliği Artırma**
- **Veri Merkezlerini İşletmeyi ve Bakımını Durdurma**
- **Dakikalar İçinde Küreselleşme:** AWS'nin küresel altyapısını kullanın.
### Bulutun Çözdüğü Problemler

- **Esneklik:** Gerektiğinde kaynak türlerini değiştirebilme.
- **Maliyet Etkinliği:** Kullandığınız kadar ödeme yapma.
- **Ölçeklenebilirlik:** Daha büyük yükleri karşılamak için donanımı güçlendirme veya ek düğümler ekleme.
- **Esneklik:** Gerektiğinde genişleme veya küçülme yeteneği.
- **Yüksek Erişilebilirlik ve Hata Toleransı:** Veri merkezleri arasında yedekleme.
- **Çeviklik:** Yazılım uygulamalarını hızla geliştirme, test etme ve başlatma.
### Bulut Bilişim Türleri

- **Altyapı Hizmeti (IaaS)**
  - Bulut BT için yapı taşları sağlar.
  - Ağ, bilgisayarlar, veri depolama alanları sağlar.
  - En yüksek düzeyde esneklik sağlar.
  - Geleneksel yerel BT ile kolayca paralel çalışabilir.
- **Platform Hizmeti (PaaS)**
  - Temel altyapıyı yönetme ihtiyacını ortadan kaldırır.
  - Uygulamalarınızı dağıtma ve yönetmeye odaklanın.
- **Yazılım Hizmeti (SaaS)**
  - Tamamlanmış bir ürün olup, hizmet sağlayıcı tarafından çalıştırılır ve yönetilir.
### Bulut Bilişim Türlerine Örnekler

- **Altyapı Hizmeti:**
  - Amazon EC2 (AWS üzerinde)
  - GCP, Azure, Rackspace, Digital Ocean, Linode
- **Platform Hizmeti:**
  - Elastic Beanstalk (AWS üzerinde)
  - Heroku, Google App Engine (GCP), Windows Azure (Microsoft)
- **Yazılım Hizmeti:**
  - Birçok AWS hizmeti (örneğin: Makine Öğrenmesi için Rekognition)
  - Google Apps (Gmail), Dropbox, Zoom
### Bulutun Fiyatlandırması - Hızlı Bakış

- AWS'nin, kullanım başına ödeme modelini takip eden 3 temel fiyatlandırma prensibi vardır.
- **İşlem:** 
  - İşlem süresi için ödeme yapın.
- **Depolama:** 
  - Bulutta depolanan veri için ödeme yapın.
- **Veri çıkışı:** 
  - Buluttan veri çıkışı ücretlendirilir. Veri girişi ücretsizdir.
- Geleneksel BT'nin pahalı sorununu çözer.
### AWS Bulut Kullanım Alanları

- AWS, sofistike ve ölçeklenebilir uygulamalar oluşturmanıza olanak tanır.
- Çeşitli endüstriler için geçerlidir.
- Kullanım alanları şunlardır:
  - Kurumsal BT, Yedekleme ve Depolama, Büyük Veri Analitiği
  - Web sitesi barındırma, Mobil ve Sosyal Uygulamalar
  - Oyun
## AWS Küresel Altyapısı

- AWS Bölgeleri
- AWS Erişilebilirlik Bölgeleri
- AWS Veri Merkezleri
- AWS Uç Noktaları / Erişim Noktaları
- <https://infrastructure.aws/>
### AWS Bölgeleri

- AWS'nin dünya genelinde bölgeleri vardır.
- İsimler us-east-1, eu-west-3 vb. olabilir.
- Bir bölge, bir **veri merkezi kümesidir.**
- **Çoğu AWS hizmeti bölge bazlıdır.**
### AWS Bölgesi Nasıl Seçilir?

Yeni bir uygulama başlatmanız gerektiğinde nerede yapmalısınız?

- **Veri yönetimi ve yasal gereksinimlerle uyum:** Veriler, sizin açık izniniz olmadan bir bölgeden çıkmaz.
- **Müşterilere yakınlık:** Gecikmeyi azaltır.
- **Bir Bölgede mevcut hizmetler:** Yeni hizmetler ve yeni özellikler her bölgede mevcut değildir.
- **Fiyatlandırma:** Fiyatlar bölgeden bölgeye değişir ve hizmet fiyatlandırma sayfasında şeffaftır.
### AWS Erişilebilirlik Bölgeleri

- Her bölge genellikle 3 erişilebilirlik bölgesine sahiptir (minimum 2, maksimum 6). 
- Örnek:
  - ap-southeast-2a
  - ap-southeast-2b
  - ap-southeast-2c
- Her erişilebilirlik bölgesi (AZ), yedekli güç, ağ ve bağlantıya sahip bir veya daha fazla ayrı veri merkezidir.
- Felaketlerden izole olmaları için birbirlerinden ayrıdırlar.
- Yüksek bant genişliğine sahip, ultra düşük gecikmeli ağ bağlantılarıyla birbirlerine bağlıdırlar.
### AWS Uç Noktaları (Edge Locations)

- Amazon'un 42 ülkede 84 şehirde 216 Uç Noktası (205 Edge Location ve 11 Bölgesel Önbellek) bulunmaktadır.
- İçerik, son kullanıcılara daha düşük gecikmeyle iletilir.
## AWS Konsolu Turu

- **AWS'nin Küresel Hizmetleri:**
  - Kimlik ve Erişim Yönetimi (IAM)
  - Route 53 (DNS hizmeti)
  - CloudFront (İçerik Dağıtım Ağı)
  - WAF (Web Uygulama Güvenlik Duvarı)
- **Çoğu AWS hizmeti bölge bazlıdır:**
  - Amazon EC2 (Altyapı Hizmeti)
  - Elastic Beanstalk (Platform Hizmeti)
  - Lambda (Fonksiyon Hizmeti)
  - Rekognition (Yazılım Hizmeti)
- **Bölge Tablosu:** <https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services>
## Paylaşımlı Sorumluluk Modeli

- MÜŞTERİ = BULUT İÇİNDE GÜVENLİKTEN SORUMLULUK
- AWS = BULUTUN GÜVENLİĞİNDEN SORUMLULUK
* * *

