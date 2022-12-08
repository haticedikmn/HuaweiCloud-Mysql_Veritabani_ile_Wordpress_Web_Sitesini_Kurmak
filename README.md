# Huawei Cloud Mysql Veritabani ile Wordpress Web Sitesini Kurmak

Bu yazımızda Cloud Container Engine üzerinde Mysql veritabanı sunucusu ve Wordpress web sitesi geliştireceğiz.

### Bulut Konteyner Motoru (CCE) Hizmeti:
Konteynerli uygulamalar oluşturmanız, çalıştırmanız ve ölçeklendirmeniz için barındırılan bir Kubernetes hizmeti.

### Virtual Private Cloud (VPC): 
Sanal Özel Bulut (VPC), çevrimiçi kaynakları sanal özel ağlarla izole etmenizi sağlar. VPC, bulut kaynaklarınızın birbirleriyle, internetle ve şirket içi ağlarla güvenli bir şekilde iletişim kurmasını sağlar.

### SoftWare Repository for Container (SWR):
Konteyner görüntülerinin tüm yaşam döngüsünü kolayca yönetmenize olanak tanır ve uygulamalarınız için görüntülerin güvenli bir şekilde dağıtılmasını kolaylaştırır.

### 1. CCE kümesi için VPC oluşturma

İlk olarak 1 tane vpc kurarak işleme başlıyoruz.

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/1.png)<br/><br/>

### 2. CCE Kümesi Oluşturma

Sonrasında ise 1 tane CCE kümesi oluşturarak devam ediyoruz.

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/2.png)<br/><br/>

### 3. CCE Küme Düğümü Oluşturma

CCS-demo >> nodes >> create node diyerek düğümü oluşturabilirsiniz.

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/3.png)<br/><br/>

### 4. Mysql Sunucu konteyneri oluşturma (StatefulSet)

CCE-demo >> workloads >> statefulsets >> create workload diyerek oluşturabilirsiniz.

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/4.png)<br/><br/>

### 5. Wordpress docker görüntüsünü SWR hizmetine yükleme

Adım 1 Aşağıdaki görüntüyü yerel bilgisayarınıza indirin 

https://articleimages.obs.ap-southeast-3.myhuaweicloud.com:443/Articles/docker-images/wordpress.tar 

SWR servis bağlantısına tıklayın https://console-intl.huaweicloud.com/swr/ 

'Resim Yükle' düğmesine tıklayın 

Bundan sonra indirilen wordpress.tar dosyasını seçin ve yükleyin.

### 6. Wordpress Web Sitesi konteyneri oluşturma (Deployment)

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/5.png)<br/><br/>

### 7. Wordpress Web Sitesini Yapılandırma

Karışınıza çıkan sitede siteyi açmak istediğiniz dili seçerek ilerleyebilirsiniz ve daha sonrasında bir giriş ekranı ile karşılasacaksınız o aşamayı da bilgilerinizi girerek
tamamlarsanız WordPrees adımına gelebilirsiniz ve istediğiniz içerikte web sitenizi oluşturabilirsiniz. 

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/6.png)<br/><br/>

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/7.png)<br/><br/>

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/8.png)<br/><br/>

![This is an image](https://github.com/haticedikmn/HuaweiCloud-Mysql_Veritabani_ile_Wordpress_Web_Sitesini_Kurmak/blob/main/img/9.png)<br/><br/>


# Son


