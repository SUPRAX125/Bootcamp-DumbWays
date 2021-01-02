# 01
DevOps adalah sebuah kultur atau budaya yang diawali dengan melakukan sharing ilmu dalam teknologi informasi yang membahas permasalahan dan solusi yang terjadi pada development dan juga operation. Namun seiring berjalannya waktu, DevOps menjadi posisi perusahaan yang menjembatani dan membuat stabilitas antara developer dan juga operation. DevOps membuat developer dapat bekerja secara berulang untuk melakukan update pada sistem dan operation dapat membuat sistem secara stabil tanpa adanya gangguan.

Penerapan pemikiran sistem DevOps adalah.

1.  Melakukan sharing untuk menyelesaikan permasalahan
    
2.  Membuat proses CICD, ITSM, Lean, dan, Agile
    
3.  Membuat Automation deployment
    

Pada dasarnya, DevOps merupakan istilah yang terdiri dari CALMS yaitu Culture merupakan suatu budaya , Automation yaitu membuat sistem automasi agar dapat mendeploy secara otomatisasi, Lean yaitu membagi masalah menjadi masalah-masalah kecil agar dapat diselesaikan dengan mudah, Measurement yaitu membuat suatu pengukuran kinerja sistem, dan Sharing yaitu melakukan sharing ilmu. Seorang DevOps untuk menyelesaikan permasalah diperlukan perencanaan, perencanaan DevOps dilihat dari tiga aspek, yaitu.

1.  Why, membahas tujuan dan sebab alasan dari adanya sistem tersebut.
    
2.  How, membahas bagaimana cara kerjanya.
    
3.  What, membahas apa yang akan dilakukan.
    

DevOps memiliki 3 prinsip yang disebut The Three Ways, prinsip-prinsip tersebut ialah.

1.  Flow, melakukan pekerjaan dari tahap A ke tahap B
    
2.  Feedback, membuat satu siklus pekerjaan
    
3.  Continuous Experimentation and Learning, membuat siklus berulang didalam flow pekerjaan.
    

Dalam DevOps, tugas-tugas tersusun secara transparan. Setiap tugas yang dibagi-bagi menjadi pekerjaan kecil akan disusun ke dalam kanban, sehingga tugas dapat disusun dalam beberapa bagian yaitu.

1.  Backlog, tugas-tugas yang tersedia.
    
2.  Planning, tugas yang akan dikerjakan.
    
3.  On Progress, tugas yang sedang dikerjakan.
    
4.  On Review, tugas yang sedang diperiksa.
    
5.  Done, tugas yang sudah selesai dikerjakan.
    

Jadi, dapat disimpulkan ialah DevOps merupakan pekerjaan yang mengintegrasi developer agar dapat melakukan update secara berkala dan operation agar sistem dapat stabil walaupun developer selalu melakukan update, namun dikarenakan DevOps awal dari kultur berkumpul dan sharing-sharing sehingga dalam DevOps akan selalu dilakukan pertemuan untuk sharing-sharing ilmu.

  

Dan untuk flow DevOps ialah diawali dari Development yang difungsikan sebagai testing untuk para developer dalam memeriksa script yang telah dibuat. Biasanya dalam tahap development, service disebut sebagai Alpha. Urutannya ialah sebagai berikut.

1.  Developer melakukan git push, lalu mendapat trigger berupa push yang akan dijalankan oleh Jenkins (CI/CD)
    
2.  Lalu Jenkins melakukan checkout pada branch ‘dev’ yang dimana Jenkins sudah mengarah kepada service yang ditaruh url repository git
    
3.  Setelah itu melalui Unit Test, untuk dilakukan testing terhadap unit-unit keseluruhan kode perangkat lunak, seperti function, interface, class, dan lain-lain
    
4.  Lalu Code Review dengan Sonarqube, digunakan untuk melakukan scanning script untuk melihat smell code, bugs, vulnerability, dan lain-lain untuk mencapai representasi clean code
    
5.  Lalu melalui proses build service dengan Docker yang dimana sudah dibuat Dockerfile
    
6.  Lalu service yang sudah dibuild akan dilakukan pembentukan chart dengan Helm Chart
    
7.  Helm chart yang sudah dibentuk akan di push ke artifactory untuk menyimpan data tsb di dalam suatu sistem
    
8.  Lalu deployment dengan Kubernetes
    
9.  Terakhir, akan masuk notifikasi melalui Jira
    

Setelah semua code telah settle untuk dilakukan testing, maka service akan melalui Staging yaitu melakukan testing automation untuk dapat mencoba aplikasi langsung sebelum digunakan oleh end user. Biasanya Staging berada pada versi Beta. Urutannya ialah.

1.  Sama seperti dev, sampai service telah melalui deployment. Namun bedanya ialah disini dengan trigger merged ke staging yang sudah di approved dari gitlab
    
2.  Setelah itu dilakukan Security Test dengan Burp Suite, fungsinya adalah untuk mengetes sisi keamanan mulai dari sql injection, csrf, xss, brute force, dan beberapa vulnerability yang lain dari fitur-fitur yang disediakan Burp Suite
    
3.  Lalu dilakukan Performance Test dengan menggunakan k6, fungsinya yaitu untuk load test, ingin melihat performa API yang telah dibuat.
    
4.  Setelah itu dilakukan Functionality Test dengan Katalon, fungsinya yaitu untuk melakukan test dari segi performa, seperti yang dilakukan QA secara automate
    
5.  Lalu dari hasil-hasil tersebut akan dinotifikasi dengan Jira
    

  

Setelah semua service sudah cocok untuk digunakan oleh end user, maka service memasuki masa Production, yang dimana service akan langsung bisa digunakan oleh end user. Production sudah memasuki versi Release. Urutannya ialah.

1.  Jenkins akan menerima trigger berupa update tag release yang di mana ada pada branch master
    
2.  Setelah itu service akan dibuild dengan Helm chart yang sudah dibuat, lalu chart akan dipush ke artifactory
    
3.  Setelah itu, image service akan dibentuk tag baru dengan tag release
    
4.  Setelah itu helm chart langsung dilakukan deploy dengan kubernetes
    
5.  Terakhir mendapat notifikasi dari Jira.
