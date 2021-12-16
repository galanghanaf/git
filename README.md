# Belajar Git dan Github

## Memanggil repositori github
```bash
git clone https://github.com/(lokasi repositori)

git clone https://github.com/galanghanaf/belajar-git.git
```
## Masuk kedalam repositori github
```
cd /belajar-git
```
## Membuat folder dalam folder belajar-git
```
mkdir git
```
## Membuat file dalam folder belajar-git/git/
```
touch git/index.html

touch git/index.js

touch git/main.css
```

## Mengecek status git
```
git status
```
## Setelah itu lakukan git add pada file, bisa spesifik atau seluruhnya
```
git add <namafile>

git add .
```
## Selajutnya lakukan commit
```
git commit -m '<jelaskan aktivitas yang diubah>'

git commit -m 'menambahkan file'
```