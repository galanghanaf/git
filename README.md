# Tutorial Git dan Github

## Konfigurasi git
#### Konfigurasi nama
```
git config --global user.name 'nama'
```
- contoh
```
git config --global user.name 'Galang Hanafi'
```

#### Konfigurasi email
```
git config --global user.email 'nama@email.com'
```
- contoh
```
git config --global user.email 'galanghanafi8@gmail.com'
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
git commit -m 'deskripsikan aktivitas yang dilakukan'
```
- contoh
```
git commit -m 'menambahkan file'
```

## Apabila kita salah mendeskripsikan aktivitas pada commit, kita tetap bisa mengubah deskripsi aktivitas, namun cara ini hanya bekerja pada commit terbaru
```
git commit --amend -m 'menambahkan file index.html'
```

## Melihat history commit
```
git log
```
setelah itu akan muncul tampilan seperti dibawah ini
```
commit 4jf233a1a6ac8fac081fdc6e3873ccd1li7da5cb (HEAD -> main, origin/main, origin/HEAD)
Author: galanghanafi <galanghanafi8@gmail.com>
Date:   Fri Dec 17 18:58:27 2021 +0700

    update index.js
```

## Melihat perubahan dari isi hash commit
```
git show <kode hash commit>
```
- contoh
```
git show 4jf233a1a6ac8fac081fdc6e3873ccd1li7da5cb
```
setelah itu akan muncul tampilan seperti dibawah ini
```
commit d73233a1a6ac8fac0816206e3873ccd1a3fda5cb (HEAD -> main, origin/main, origin/HEAD)
Author: galanghanafi <galanghanafi8@gmail.com>
Date:   Fri Dec 17 18:58:27 2021 +0700

    update index.js

diff --git a/index.js b/index.js
index e69de29..2ac23f8 100644
--- a/index.js
+++ b/index.js
@@ -0,0 +1 @@
+console.log("halo git");
\ No newline at end of file
```

## Melakukan push ke github
```
git push -u origin main
```

## Melakukan pull ke github
```
git pull
```

## Cara membuat branch
```
git branch <nama>
```
- contoh
```
git branch project_a
```

## Melihat total branch di lokal
```
git branch
```

## Melihat total branch di github
```
git branch -r
```

## Melakukan push branch ke github
```
git push -u origin <nama_branch>
```
- contoh
```
git push -u origin project_a
```

## Switch branch
```
git checkout project_a
```

## Kembali ke branch utama
```
git checkout main
```

## Cara merge branch project_a ke main
```
git checkout main
```
- Optional
```
git merge project_a
```
- ### Paling Disarankan
```
git merge --squash project_a
```