Cara configurasi git
	git config --global user.name "nama user"
	git config --global user.email namaemail
Cara mengetahui configurasi git
	git config --list

1. Membuat Repositori
	git init nama_proyek
2. Melihat status git 
	git status
3. Membuat revisi
	a. kondisi Modified ketika file ditambahkan ke dalam proyek
	b. Membuat kondisi menjadi stagged
		git add nama_file
	c. Commited 
		git commit -m "nama perubahan"
4. Melihat log revisi
	a. melihat semua log
		git log
	b. log lebih pendek
		git log --oneline
	c. log pada nomer revisi/commit
		git log nomorrevisi
	d. log pada file tertentu
		git log nama_file
	e. log yang dilakukan author tertentu
		git log --author='nama_author'
5. Melihat perbandingan revisi
	a. melihat perbandingan pada file tertentu
		git diff namafile
	b. melihat perbandingan antar revisi/commit
		git diff nomerrevisi1 nomorrevisi2
	c. melihat perbandingan antar cabang
		git diff namacabang1 nama cabang2
6. Membatalkan perubahan 
	a. jika kondisi sedang modified
		git checkout namafile
	b. jika kondisi sudah dalam keadaaan staged/ sudah di add
		- kita harus mengubahnya ke dalam kondisi modified
			git reset namafile
		-lalu jika sudah dalam keadaan modified kita batalkan
			git checkout namafile
	c. jika kondisi sudah commit
		-kita kembalikan dulu kondisi file ke commit sebelumny
			git checkout nomorcommitsebelumnya namafile
		-lalu kita kembalikan dalam kondisi modified
			git reset namafile
	d. kembali ke 3 commit sebelumnya
		git checkout HEAD~3 namafile
	e. membatalkan semua perubahan yang ada
		git revert -n nomorcommit
7. Menggunakan percabangan
	a. membuat cabang baru
		git branch namacabang
	b. melihat caban branch yang ada
		git branch
	c. berpindah cabang/branch
		git checkout branchyangdituju
	d. Menggabungkan cabang
		git merge namacabang
	e. menghapus cabang 
		git branch -d namacabang
