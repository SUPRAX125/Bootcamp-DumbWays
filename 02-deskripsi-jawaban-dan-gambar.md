## AWS

AWS (Amazon Web Services) merupakan penyedia layanan jasa Cloud Computing dimana kita akan disediakan infrastruktur
yang disediakan oleh Amazon, sehingga kita tinggal menggunakan beberapa komponen seperti virtual machine, server, network, dan lain-lain.
AWS menyediakan layanan Public Cloud. Beberapa service yang disediakan AWS ialah.

**- Compute**

Service ini ialah untuk keperluan komputasi dalam AWS seperti manajement Virtual Server, Bare Metal Server untuk server fisik,
container dan juga Virtual Private Server.

**- Storage**

Service ini untuk media penyimpanan AWS dengan beberapa data yang akan diolah dari aplikasi yang dinaikan dari AWS.
Fitur yang dimiliki ialah Object Storage, Storage untuk VM, File Storage, dan lain sebagainnya.

**- Database**

AWS menyediakan layanan untuk koneksi dengan database, untuk jenis database seperti Relational Database dan Non Relational,
Timeseries Database, Data Warehousing untuk Big Data, dan juga In-Memory Data Store untuk managemen memory cache

**- Migration Service**

Service ini banyak dimiliki AWS seperti migrasi untuk Database, Server, dan data skala kecil maupun besar.

**- Networking & Content Delivery**

AWS memiliki fitur untuk konfigurasi jaringan yang ada pada cloud computing ini. Bisa membuat suatu jaringan untuk 
VPC (Virtual Private Cloud), Network Gateway, CDN (Content Delivery Network), Load Balancer, dan lain-lain
# 



## OpenStack

OpenStack merupakan Software Open Source untuk membangun Cloud Computing dan berbasis IaaS juga, sama seperti AWS dan dibuat oleh
Rackspace Hosting dan bersana NASA pada tahun 2010. Openstack banyak didukung oleh beberapa perusahaan seperti Ciscon,
IBM, HP, dan juga Dell. Beberapa perusahaan tersebut sudah memiliki Plugin untuk bisa diintegrasikan ke OpenStack. Lalu OpenStack juga
merupakan jenis Hybrid Cloud yaitu bisa menjadi Private Cloud dan juga Public Cloud. Komponen yang dimiliki Oleh OpenStack ialah.

**- Nova**

Untuk komponen Compute. Nova merupakan komponen untuk mengatur proses dan alokasi CPU untuk 
setiap virtual machine. Kontroler compute seperti Nova, merupakan komponen utama dari 
sistem IaaS, karena entitas ini yg mengatur proses dan alokasi CPU untuk setiap VM.


**- Cinder**

Untuk Block Storage. Cinder merupakan komponen storage yang digunakan oleh element 
compute (Nova). Cinder memberikan akses kepada admin untuk mengatur kebutuhan terhadap 
media penyimpanan. Cinder melakukan virtualisasi terhadap kumpulan dari perangkat block 
storage dan memberikan akses kepada elemen compute untuk menggunakan resource tersebut 
tanpa perlu tahu storage mana yang sedang digunakan.


**- Quantum (Neutron)**

Neutron (sebelumnya disebut quantum) merupakan komponen untuk menyediakan Network 
connectivity as a service i.e. Neutron melakukan kendali atas network yang melibatkan 
virtual machine. Fungsi yang termasuk di dalamnya adalah mengatur jaringan atau 
subnet, router, load-balancer, gateway, dan floating IP. Neutron juga merupakan 
elemen yg (akan) banyak bersentuhan dengan konsep SDN.

**- Glance**

Layanan ini menyimpan dan menyediakan virtual machine image yang bisa 
digunakan sebagai boot record oleh virtual machine, image juga bisa masukan ke dalam block storage.

**- Swift**

Untuk komponen Object Storage. Swift merupakan komponen Object Storage pada Openstack. Swift dapat menyimpan 
dan menerima data yang sangat banyak dan dapat di-scale dengan mudah. Switch ideal untuk menyimpan 
data tidak terstruktur yang dapat berkembang tanpa batas.

**- Keystone**

Disebut dengan keystone karena digunakan sebagai autentikasi setiap user dan service. Untuk Identity Service

**- Horizon**

Untuk tampilan Dasboard. Horizon menyediakan antarmuka web untuk semua komponen dalam Openstack termasuk 
Nova, Swift, Keystone dll. Horizon merupakan implementasi (resmi untuk konsep) dashboard OpenStack. 
Layanan OpenStack Horizon dibuat menggunakan platform Django dengan konsep yg extensible dan mengunakan komponen-komponen reusable.

**- Heat**

Heat merupakan project utama untuk orchestration. Program orchestration merupakan penengah antara 
manusia dan mesin yang digunakan mengatur semua komponen infrastruktur dan aplikasi di dalam cloud Openstack.

**- Trove**

Trove merupakan komponen Database-as-a-service untuk Openstack. User atau administrator 
database dapat mengatur beberapa database instance sesuai kebutuhan.

**- Ceilometer**

Layanan untuk memonitor dan mengukur billing, benchmark, skalabilitas, dan statistik proses pada cloud.

>Note:
>
>Namun untuk perbedaan yang jelas antara OpenStack dan AWS ialah dari fitur yang dimilik. AWS memiliki fitur yang banyak
>dibandingkan dengan OpenStack, service yang saya jelaskan di atas untuk AWS hanya sebagian kecil, AWS masih memiliki banyak
>fitur. Dan perbedaan yang sangat jelas ialah dari segi budget bahwa OpenStack lebih murah ketimbang AWS dikarenakan Openstack
>yaitu Open Source yang di mana jelas bahwa Open Source itu murah, dan memang fitur AWS lebih banyak sehingga itu juga yang membuat
>AWS mahal.
