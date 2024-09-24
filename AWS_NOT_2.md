# 🌩️ AWS Certified Cloud Practitioner - Hızlı Hazırlık Notları

Bu notlar, AWS Cloud Practitioner sınavına hazırlanırken en önemli konuları özetler. Bilgileri birkaç kez gözden geçirerek sınavda başarılı olabilirsin.

---

## 📚 1. Bulut Bilişim Temelleri

- **Bulut Bilişim Nedir?**: İnternet üzerinden sunuculara, veritabanlarına, ağ altyapısına ve diğer bilişim kaynaklarına erişim sağlama.
- **AWS’nin Temel Avantajları**:
  - 💸 **Kullandıkça Öde (Pay-as-you-go)**: Sadece kullandığın kadar ödeme yap.
  - 🛠️ **Esneklik (Flexibility)**: Kaynakları ihtiyacına göre ölçekle.
  - ⚡ **Hız ve Çeviklik (Speed and Agility)**: Dakikalar içinde kaynakları başlat.
  - 🌍 **Küresel Erişim (Global Reach)**: AWS'nin dünya çapındaki veri merkezlerinden yararlan.

---

## 💻 2. AWS Hizmet Kategorileri

### 2.1. Hesaplama (Compute)
- **Amazon EC2**: Ölçeklenebilir sanal sunucular.
  - *Kullanım Senaryoları*: Web uygulamaları, veritabanı sunucuları.
- **AWS Lambda**: Sunucusuz, yalnızca kod çalıştırmaya odaklanılan hizmet.
  - *Avantajı*: Sunucu yönetimine gerek yok; sadece çalıştırılan süre için ödeme yapılır.
  
### 2.2. Depolama (Storage)
- **Amazon S3 (Simple Storage Service)**: Yüksek dayanıklılığa sahip nesne depolama.
  - *Özellikler*: 11 9'luk veri dayanıklılığı (99.999999999%).
- **Amazon EBS (Elastic Block Store)**: EC2 örnekleri için blok depolama.
  - *Kullanım*: Veritabanları, uygulama sunucuları.
- **Amazon Glacier**: Uzun süreli veri arşivleme için düşük maliyetli depolama.

### 2.3. Veritabanı (Database)
- **Amazon RDS (Relational Database Service)**: Yönetilen ilişkisel veritabanı hizmeti (MySQL, PostgreSQL, SQL Server, vb.).
  - *Özellik*: Yedekleme, yama yönetimi, otomatik ölçekleme.
- **Amazon DynamoDB**: Tamamen yönetilen NoSQL veritabanı.
  - *Özellik*: Milisaniyelik gecikme, otomatik ölçekleme.

### 2.4. Ağ ve İçerik Dağıtımı (Networking & Content Delivery)
- **Amazon VPC (Virtual Private Cloud)**: İzole edilmiş sanal ağ; ağ yapılandırması üzerinde tam kontrol.
- **Amazon Route 53**: DNS ve alan adı yönlendirme hizmeti.
- **Elastic Load Balancer (ELB)**: Yükü birden fazla sunucuya otomatik olarak dağıtır.
- **Amazon CloudFront**: Düşük gecikme ile hızlı içerik dağıtımı için CDN hizmeti.

---

## 🔒 3. Güvenlik ve Uyumluluk

- **Paylaşımlı Sorumluluk Modeli (Shared Responsibility Model)**:
  - 🔐 **AWS'nin Sorumluluğu**: Fiziksel altyapının güvenliği (veri merkezi).
  - 🛡️ **Müşterinin Sorumluluğu**: Uygulama, veri ve erişim yönetimi.
- **IAM (Identity and Access Management)**: Kullanıcı erişim haklarını yönetme.
  - *Özellikler*: Roller, ilkeler ve gruplar oluşturma.
- **MFA (Multi-Factor Authentication)**: Hesaplar için iki faktörlü kimlik doğrulama.
- **AWS Shield**: DDoS saldırılarına karşı koruma sağlar.
- **AWS WAF (Web Application Firewall)**: Web uygulamalarına yönelik saldırılara karşı koruma.

---

## 💵 4. Fiyatlandırma ve Maliyet Yönetimi

### 4.1. Fiyatlandırma Modelleri
- **Kullandıkça Öde**: Kaynakları kullandığın kadar ödeme yaparsın.
- **Rezerve Edilmiş Örnekler (Reserved Instances)**: Uzun vadeli taahhütlerle maliyetleri düşürebilirsin.
- **Spot Örnekler (Spot Instances)**: Kullanılmayan EC2 kapasitesiyle daha düşük maliyetler.

### 4.2. AWS Free Tier
- **Ücretsiz Katman (Free Tier)**: Yeni kullanıcılar için belirli AWS hizmetleri 12 ay boyunca ücretsizdir.
  - *Örnek*: Amazon S3’te 5 GB ücretsiz depolama, Amazon EC2’de ayda 750 saatlik ücretsiz kullanım.

### 4.3. Maliyet Yönetimi Araçları
- **AWS Pricing Calculator**: Kullanım maliyetlerini önceden tahmin etme aracı.
- **AWS Cost Explorer**: Harcamalarını analiz etmek ve gelecekteki maliyetleri tahmin etmek için kullanılır.

---

## 🏗️ 5. AWS Mimarisi ve Yüksek Erişilebilirlik

- **Yüksek Erişilebilirlik (High Availability)**: Kaynaklar, farklı AWS bölgelerinde dağıtılır ve kesintisiz hizmet sağlar.
- **Auto Scaling**: Uygulamalarını otomatik olarak ölçeklendirme (ihtiyaç arttığında yeni sunucular başlatılır, düştüğünde durdurulur).
- **CloudFront**: İçerik dağıtım ağı (CDN) ile düşük gecikme ve yüksek hız sağlar.

---

## 📊 6. AWS Yönetim ve İzleme Araçları

- **Amazon CloudWatch**: AWS kaynaklarını izler, metrikler toplar ve uyarılar oluşturur.
- **AWS CloudTrail**: AWS'deki API çağrılarını izleyerek denetim ve uyumluluk sağlar.
- **AWS Trusted Advisor**: Güvenlik, performans, maliyet optimizasyonu ve kullanılabilirlik konularında önerilerde bulunur.
- **AWS CloudFormation**: Altyapıyı kod olarak tanımlamaya ve yönetmeye olanak tanır (Infrastructure as Code).

---

## 🚀 7. AWS'nin Temel Hizmetleri

- **Elastic Load Balancer (ELB)**: Trafiği sunucular arasında dengeler.
- **Amazon CloudFront**: Global içerik dağıtımı sağlar.
- **Amazon S3**: Güvenli, ölçeklenebilir ve düşük maliyetli depolama çözümü.

---

## 🎯 8. Sınav Bilgileri

- **Süre**: 90 dakika.
- **Soru Sayısı**: Yaklaşık 65 çoktan seçmeli soru.
- **Geçme Notu**: 1000 üzerinden 700 puan.
- **Soru Tipleri**: Temel AWS hizmetleri, fiyatlandırma, güvenlik, en iyi uygulamalar üzerine kavramsal ve teknik sorular.

---

Bu notlar sınav için gerekli tüm bilgileri içerir. AWS Cloud Practitioner sınavına hazırlanırken odaklanman gereken konuları kısa, öz ve etkili bir şekilde gözden geçirebilirsin. Başarılar! 🚀
