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
