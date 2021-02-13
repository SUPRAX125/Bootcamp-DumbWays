#Dokumentasi Learning Git 

Git merupakan suatu aplikasi untuk Version Control System sebagai repository suatu project untuk menyimpan script yang dimana project tersebut akan dikerjakan bersama-sama oleh sekumpulan programmer
tanpa adanya saling menunggu sehingga project tersebut terintegrasi dalam satu platform. Git memiliki fitur yaitu mentraking bahwa script tersebut siapa yang edit, delete, dan adding. Lalu untuk melakukan proses penaikan
aplikasi dari deployment, staging, dan production diperlukan Git.

Dokumentasi Learning Git
Berikut beberapa perintah yang ada pada Git

**- git init**
Untuk inisialisasi folder/lokal yang akan diupload ke git

**- git remote add https://gitlab.com/devops-klik/onboarding/learning-git.git**
Untuk mengkoneksikan lokal ke repository

**- git add First.txt**
Memilih file/folder untuk ditambahkan ke repository

**- git commit -m “first commit**
Menambahkan catatan/detail file yang telah diupload

**- git push origin master**
Upload file/folder yang telah diadd atau update kegiatan yang ada di lokal

**- git pull origin master**
Memperbaharui file/folder yang ada di lokal dengan mengambil dari repository

**- git branch**
Melihat branch yang terbentuk di lokal dan melihat sedang berada di branch mana

**- git branch -va**
Melihat semua branch yang terbentuk sampai branch yang ada di repository

**- git branch Feature**
Membuat branch baru dengan nama Feature

**- git checkout Feature**
Pindah ke branch Feature

**- git merge origin Feature**
Menggabungkan branch Feature ke master (pindah ke branch master dahulu)

**- git branch -D Feature**
Menghapus branch Feature yang ada di lokal (pindah ke branch lain dahulu)

**- git push origin --delete Feature**
Menghapus branch Feature yang ada di repository

**- git push**
Untuk mengembalikan kesemula, jika sudah dilakukan perubahan namun tidak jadi

**- git revert HEAD**
Ingin melakukan pembatalan commit, otomatis membuka file (vim) report pembatalan commit

**- git revert HEAD --no-edit**
Pembatalan commit tanpa membuka file report pembatalan commit

**- git reset HEAD .**
Mengembalikan seperti semula pada saat ada perubahan

**- git reset --hard**
Mengembalikan seperti semula dan kembali ke branch master
