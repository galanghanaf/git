# Tutorial Git dan Github

## Konfigurasi git
#### Konfigurasi nama
```
git config --global user.name "nama"
```
- contoh
```
git config --global user.name "Galang Hanafi"
```
#### Konfigurasi email
```
git config --global user.email "nama@email.com"
```
- contoh
```
git config --global user.email "galanghanafi8@gmail.com"
```
## Melihat hasil konfigurasi git
```
git config -l
```

## Memanggil repositori github
```
git clone https://github.com/lokasi-repositori
```
- contoh
```
git clone https://github.com/galanghanaf/belajar-git.git
```
## Masuk kedalam repositori github
```
cd ./belajar-git
```

## Membuat file
```
touch index.html
```
```
touch index.js
```
```
touch main.css
```

## Mengecek status git
```
git status
```
## Setelah itu lakukan git add pada file, bisa spesifik atau seluruhnya
```
git add <namafile>
```
- contoh add spesifik file
```
git add index.html
```
- contoh add seluruh file
```
git add .
```
## Apabila tidak jadi melakukan git add, maka dapat dikembalikan ke keadaan sebelum di git add
```
git restore --staged <namafile>
```
- contoh
```
git restore --staged index.html
```
## Selajutnya lakukan commit
```
git commit -m 'jelaskan aktivitas yang dilakukan'
```
- contoh
```
git commit -m 'menambahkan file'
```

## Melihat history commit
```
git log
```