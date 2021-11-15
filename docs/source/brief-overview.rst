Penjelasan Singkat Model Informasi SDMX
=======================================

Cakupan Permasalahan
--------------------

Pernyataan Masalah Secara Singkat
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Suatu sistem statistik terdiri dari banyak sub sistem dan komponen. Persoalan utama sistem komputer termasuk sistem statistik adalah sistem —atau dapat disebut perangkat lunak— dibangun secara silo atau setidaknya dibangun dengan komponen yang tidak independen dan tidak dapat digunakan kembali.

Pertimbangkan alur proses sederhana berikut ini, yaitu alur impor data ke basis data dan alur diseminasi data.

**Alur Impor Data**

.. image:: images/img1.png

**Alur Diseminasi Data**

.. image:: images/img2.png

Berikut adalah beberapa kelemahan yang kemungkinan terdapat di dalam sistem yang saat ini mendukung proses tersebut.

Desain Basis Data
-----------------

Skema basis data dirancang secara internal sehingga dapat menampung semua data yang dikerjakan di dalam suatu departemen (selanjutnya akan disebut institusi). Institusi dapat memutuskan untuk mengadopsi basis data Oracle, dan tabel basis data disesuaikan untuk menyimpan data spesifik yang relevan sesuai dengan cakupan tempat institusi bekerja. Tidak perlu menggunakan lebih dari 2 bahasa, setiap tabel berisi label khusus untuk setiap bahasa di mana pun data tersebut muncul.

Ada satu tabel basis data yang besar berisi nilai observasi untuk setiap dataset. Ada banyak tabel basis data terkait yang berisi informasi lebih lanjut tentang pengamatan. Tabel tertaut digunakan untuk memfasilitasi pemfilteran saat membuat kueri basis data. Data dan informasi di dalam tabel tersebut berguna untuk menyusun hasil kueri yang akan disajikan kepada pengguna.

Impor Data
----------

Institusi menerima data dari banyak organisasi penyedia data, dan dengan demikian format data di setiap dataset bergantung pada organisasi pengirim. Pengimpor data dicatat untuk mendukung dokumentasi ketika terdapat penawaran data. Dalam beberapa situasi, tabel pemetaan perlu didefinisikan untuk memetakan klasifikasi klien ke pemetaan yang digunakan di internal institusi. Terdapat suatu aturan validasi yang ditetapkan untuk memastikan data sesuai dengan apa yang diharapkan. Setiap importir mengimplementasikan logika validasinya sendiri. Terdapat juga validasi tambahan yang digunakan setelah data berada di dalam basis data.

Diseminasi Data
---------------

Untuk melakukan diseminasi data, tim analisis bisnis menentukan jenis kueri mana yang diperlukan. Kemudian, tim developer menulis kueri basis data untuk mendefinisikan *use cases*. *Use cases* yang didefinisikan memiliki output untuk mengekstrak dataset yang relevan. Tidak ada model formal untuk data, sehingga output sintaks bergantung pada penerima data. Jika klien baru memerlukan format output yang berbeda, tim developer akan menulis kueri basis data baru, atau mereka akan menulis transformasi dari format yang sudah ada.

Situs web dibangun di atas API yang ditentukan oleh tim analisis bisnis, dengan desainer web dan developer *backend* bekerja sama untuk membangun halaman web. Semakin banyak *use cases* yang berkembang, tim developer akan menulis API baru untuk mendukung situs web.

Secara internal, unit lain di dalam organisasi diberikan akses langsung ke tabel basis data. Unit-unit tersebut menulis logika kueri mereka sendiri berdasarkan struktur tabel untuk mendapatkan data dari sistem mereka sendiri.