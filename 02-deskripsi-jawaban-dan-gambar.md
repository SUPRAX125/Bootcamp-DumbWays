# 02
Dalam kasus ini, digunakan file .txt, untuk kasus lain bisa menggunakan ekstensi file yang lainnya.
Di sini terdapat 9 file .txt, di sini saya ingin mencari file yang dimana isi dari file tersebut yang saya ketahui hanya bertuliskan 'budi', lalu saya cari file tersebut dengan perintah

> $ grep grep -rnw *.txt -e 'budi'

Jika file lain seperti log bisa ditambahkan yaitu
> $ grep -rnw *.log-* -e '503'

Pada intinya, sintaks yang digunakan ialah
> $ grep -rnw <path/to/file/*.extension> -e '<keyword_yang_diinginkan>'

Argumen yang digunakan ilaha
**r** : recursive
**n** : menampilkan semua kata berada pada line berapa
**w** : mencocokan dengan seluruh kata
**e** : regexp
