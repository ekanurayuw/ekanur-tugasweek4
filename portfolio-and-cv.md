membuat sebuah folder kosong dengan namamu sendiri
-[ mkdir eka ]
membuat sebuah file di dalam folder tersebut dengan nama README.md, isi file tersebut dengan kalimat "Halo perkenalkan aku halaman utama"
-[touch README.md, echo -e "Halo perkenalkan aku halaman utama"]
inisialisasi folder tersebut dengan Git, kemudian simpan perubahan menggunakan commit dengan pesan "First commit"
-[git init, git commit -m "First Commit"]
Ganti teks sebelumnya dengan "Hello world"
-[nano README.md, mengganti teks, ctrl + x, enter]
Tampilkan isi teks tersebut pada command line menggunakan command cat
-[cat readme.md]
Ternyata kamu tidak ingin perubahan tersebut, dan ingin kembali ke perubahan seperti commit yang terakhir. Lakukan teknik git backtracking untuk mengembalikan ke perubahan commit yang terakhir.
-[git checkout readme.md]
buat branch baru dengan nama cv, hal ini berguna agar histori kita tidak tercampur
-[git branch cv]
pindah branch ke dalam cv, kemudian buat file dengan nama cv.txt dan isi file tersebut dengan kalimat: "Ini adalah file CV"
-[git checkout cv]
kemudian simpan perubahan menggunakan commit dengan pesan "Initial CV"
-[git commit -m "Initial CV"]
tambahkan 3 perusahaan yang akan kamu lamar, dan setiap menuliskan 1 nama perusahaan kamu harus melakukan dokumentasi dan menyimpan perubahan menggunakan commit
-[~echo -e "PT Adaro Energy Tbk (ADRO)", git commit -m "menambahkan perusahaan pertama" ~ PT Aneka Tambang Tbk (ANTM), git commit -m "menambahkan perusahaan kedua" ~ PT Astra International Tbk (ASII), git commit -m "menambahkan perusahaan ketiga"]
kembali ke branch master
-[git checkout main]
ubah file README.md menjadi "Halo perkenalkan aku halaman utama" "Ini adalah update pertama pada branch master"
-[echo -e ]
jangan lupa untuk menyimpan perubahan menggunakan commit dengan pesan "update master pertama"
-[git commit -m "update master pertama"]
gabungkan branch cv ke dalam branch master menggunakan perintah git merge
-[git merge cv]
unggah Git Repository project tersebut tersebut ke dalam GitHub
-[ git remote add https://github.com/ekanurayuw/ekanur-tugasweek4 git push] git log --graph
