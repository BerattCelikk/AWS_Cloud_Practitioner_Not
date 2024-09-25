# 🌥️ AWS Cloud Practitioner Sınavı İçin Detaylı Kapsamlı Özet

## 1. Bulut Bilişim Temelleri (Cloud Computing Basics)

### 🌐 Bulut Bilişim Nedir?
**Bulut bilişim**, internet üzerinden sunulan bilgi işlem kaynaklarının (depolama, veri işleme, sunucular vb.) kiralanmasıdır. Fiziksel altyapıya sahip olmanıza gerek kalmadan, bulut sağlayıcıları aracılığıyla hizmet alabilirsiniz. Bu model işletmelere hızlı ve esnek bir çözüm sunar.

#### **Avantajlar:**
- ⚡ **Çeviklik (Agility)**: Hızlıca kaynak ekleyip çıkarabilirsiniz.
- 🌍 **Kapsamlı Erişim (Broad Network Access)**: Hizmetlere her yerden erişim imkanı sunar.
- 💰 **Maliyet Verimliliği (Cost Efficiency)**: Yalnızca kullandığınız kaynaklar için ödeme yaparsınız.

### 🏗️ Bulut Modelleri (Cloud Deployment Models)
Bulut bilişim üç temel modelde sunulur:

- ☁️ **Kamu Bulut (Public Cloud)**: AWS, Azure, Google Cloud gibi sağlayıcıların sunduğu herkese açık bulut hizmetleridir.
- 🔒 **Özel Bulut (Private Cloud)**: Bir işletmenin kendi veri merkezlerinde oluşturduğu, sadece işletme içinde kullanılan bulut altyapısıdır.
- 🔗 **Hibrit Bulut (Hybrid Cloud)**: Kamu ve özel bulutların birleştirildiği modeldir. Kritik veriler özel bulutta tutulurken, daha genel veriler kamu bulutunda saklanabilir.

---

## 2. AWS Hizmet Modelleri (Cloud Service Models)

### 1. 🏢 IaaS (Infrastructure as a Service - Altyapı Hizmeti)
Altyapı hizmetleri, sanal sunucular, depolama alanları ve ağ kaynaklarını kiralamanıza olanak tanır. Bu modelde işletmeler donanım ile uğraşmak yerine bulut sağlayıcısından sanal makineler kiralar.

- **Örnek**: Amazon EC2 (Elastic Compute Cloud)

### 2. 🛠️ PaaS (Platform as a Service - Platform Hizmeti)
Uygulama geliştirmek için gereken altyapıyı ve yazılım geliştirme araçlarını kullanıcılara sunar. Kullanıcılar altyapı yönetmeden sadece uygulama geliştirir.

- **Örnek**: AWS Elastic Beanstalk

### 3. 📦 SaaS (Software as a Service - Yazılım Hizmeti)
Tamamen yönetilen ve kullanıma hazır yazılım çözümlerini internet üzerinden sunar. Yazılımın güncellenmesi, bakımı ve güvenliği hizmet sağlayıcısı tarafından yapılır.

- **Örnek**: Gmail, Microsoft Office 365

---

## 3. AWS'in Temel Hizmetleri (Core AWS Services)

### ⚙️ Amazon EC2 (Elastic Compute Cloud)
EC2, AWS’in sanal sunucu hizmetidir. Kullanıcılar, farklı donanım ve performans seçenekleri ile ihtiyaçlarına göre sunucular seçebilirler.

- **Instance Türleri**:
  - 🟢 **T3/M6g (General Purpose)**: Genel kullanım için dengeli işlemci ve bellek sunar.
  - 🔵 **C5 (Compute Optimized)**: Yüksek işlem gücü gerektiren uygulamalar için.
  - 🟣 **R5 (Memory Optimized)**: Bellek yoğun uygulamalar için optimize edilmiştir.

### 🗄️ Amazon S3 (Simple Storage Service)
S3, AWS’in nesne tabanlı depolama hizmetidir. Verilerinizi “bucket” adı verilen kapsayıcılarda saklar ve dünya genelinde kolay erişim sağlar.

- **S3 Bucket**: Verilerin saklandığı kapsayıcılar.
- **Depolama Sınıfları**:
  - 🌟 **S3 Standard**: Sık erişilen veriler için optimize edilmiştir.
  - 🔑 **S3 Infrequent Access (IA)**: Daha az erişilen veriler için maliyet avantajı sağlar.
  - 🧊 **S3 Glacier**: Uzun vadeli arşivleme için düşük maliyetli depolama.

### 🗄️ Amazon RDS (Relational Database Service)
RDS, AWS'in yönetilen ilişkisel veritabanı hizmetidir. Kullanıcılar yalnızca veritabanlarını yapılandırır, AWS altyapıyı yönetir.

- **Desteklenen Veritabanı Motorları**: MySQL, PostgreSQL, Oracle, SQL Server.
- ⚙️ **Multi-AZ**: Veritabanını birden fazla erişilebilirlik bölgesine yedekleyerek yüksek erişilebilirlik sağlar.

### 🌀 Amazon Lambda
Sunucusuz (serverless) bir bilgi işlem hizmeti olan Lambda, yalnızca belirli olaylar gerçekleştiğinde kod çalıştırır. Sunucu yönetimi gerekmez.

- **Kullanım Durumu**: E-posta bildirimleri, veri işleme.
- 🔗 **Event-Driven (Olay Tabanlı)**: S3'e dosya yükleme, DynamoDB değişiklikleri gibi olaylar tarafından tetiklenir.

### 🌍 Amazon CloudFront
CloudFront, AWS’in içerik dağıtım ağı (CDN) hizmetidir. Kullanıcıların içeriğini dünya çapındaki kenar noktalarından sunarak gecikmeyi azaltır ve performansı artırır.

---

## 4. AWS Güvenlik ve Kimlik Yönetimi (Security and Identity Management)

### 🔒 AWS IAM (Identity and Access Management)
IAM, AWS kaynaklarına erişimi kontrol eden bir güvenlik hizmetidir. Kullanıcılar ve roller için izinler tanımlayarak, her bir kullanıcının yapabileceklerini kısıtlayabilirsiniz.

- **IAM Policy**: Kullanıcıların hangi kaynaklara erişebileceğini ve hangi işlemleri yapabileceğini belirleyen izin kümesidir.
- **IAM Role**: AWS hizmetlerinin belirli izinlerle işlem yapmasına olanak tanır.
- 🔑 **Çok Faktörlü Kimlik Doğrulama (MFA)**: Ek güvenlik adımları ekleyerek daha güvenli erişim sağlar.

### 🗝️ AWS KMS (Key Management Service)
KMS, AWS’in sunduğu şifreleme anahtarları yönetim hizmetidir. Verilerinizi güvenli bir şekilde şifrelemek için kullanılır.

- **Kullanım Durumu**: Kritik verileri şifrelemek ve yönetmek için kullanılır.

---

## 5. AWS Fiyatlandırma ve Maliyet Optimizasyonu

### 💵 AWS Fiyatlandırma Modelleri
- ⚖️ **Kullandıkça Öde (Pay-as-you-go)**: Yalnızca kullandığınız kaynaklar için ödeme yaparsınız.
- 🔒 **Rezerve Edilmiş Fiyatlandırma (Reserved Instances)**: Uzun süreli kaynak rezervasyonu yaparak maliyet avantajı sağlarsınız.
- 💡 **Spot Instances**: AWS’in kullanılmayan kaynaklarını daha düşük maliyetle kiralayabilirsiniz, ancak bu kaynaklar AWS tarafından geri alınabilir.

### 📊 AWS Maliyet Yönetimi Araçları
- 📈 **AWS Cost Explorer**: Harcamalarınızı analiz eder ve maliyet tasarrufu fırsatlarını görmenizi sağlar.
- 💳 **AWS Budgets**: Belirli bir bütçe limiti oluşturur ve bu bütçe aşıldığında uyarılar alırsınız.

---

## 6. Yüksek Erişilebilirlik ve Olağanüstü Durum Kurtarma (High Availability and Disaster Recovery)

### 🔄 Yüksek Erişilebilirlik (High Availability)
AWS, hizmetlerinizi birden fazla **Erişilebilirlik Bölgesi (Availability Zone)** üzerinden dağıtarak yüksek erişilebilirlik sağlar. Bu sayede bir bölgede sorun olsa bile hizmetleriniz kesintisiz çalışır.

### ⚠️ Olağanüstü Durum Kurtarma (Disaster Recovery)
AWS, veri kaybını ve hizmet kesintilerini en aza indirmek için olağanüstü durum kurtarma çözümleri sunar.

- 🔥 **Sıcak Yedekleme (Hot Standby)**: Yedek sistemler sürekli aktif ve hazırdır.
- ❄️ **Soğuk Yedekleme (Cold Standby)**: Yedekler sadece gerektiğinde devreye girer, daha az maliyetlidir.

---

## 7. Veri Analitiği ve Makine Öğrenimi (Data Analytics & Machine Learning)

### 📈 Amazon Redshift
AWS'in büyük veri işleme ve veri ambarı çözümüdür. Çok büyük veri kümelerini analiz etmek ve hızlı sorgular çalıştırmak için kullanılır.

### 🧮 Amazon Athena
S3’te saklanan veriler üzerinde SQL sorguları çalıştırmak için kullanılan sunucusuz bir veri analitiği hizmetidir. Veri altyapısı yönetimi gerekmez.

### 🤖 Amazon SageMaker
Makine öğrenimi modellerini hızlıca oluşturmak, eğitmek ve dağıtmak için kullanılan bir hizmettir. Geliştiricilerin ve veri bilimcilerin, makine öğrenimi projelerini hızla başlatmasına olanak tanır.

---

## 8. AWS Küresel Altyapısı (Global Infrastructure)

### 🌍 Erişilebilirlik Bölgeleri (Availability Zones)
Her AWS bölgesi, birbirinden izole edilmiş birden fazla erişilebilirlik bölgesinden oluşur. Bu, uygulamaların yüksek erişilebilirlikle çalışmasını sağlar.

### 🏢 AWS Bölgeleri (Regions)
AWS, dünya çapında stratejik olarak yerleştirilmiş bölgelerde veri merkezleri sunar. Her bölge, bağımsız olarak yönetilen veri merkezlerinden oluşur.

---

Bu kapsamlı özet, AWS Cloud Practitioner sınavına hazırlanırken ihtiyaç duyabileceğiniz temel bilgileri ve hizmet detaylarını kapsamaktadır. 📚
