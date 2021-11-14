Kenapa Menggunakan SDMX?
========================

.. _usecases:

Mendukung untuk Beberapa *Use Cases*
------------------------------------

Pertama, penting untuk diketahui bahwa SDMX dapat memberikan lebih dari sekadar format umum bagi *data collectors* dan *data reporters* yang digunakan dalam pertukaran data dan metadata, meskipun akronimnya menggambarkan sebaliknya.

Kedua, jangan khawatir tentang bagaimana representasi sintaks dari data dan metadata. Ada banyak *tools* dan aplikasi *open source* yang dapat mengatasi kerumitan ini dan dengan demikian memungkinkan Kamu untuk menggunakan SDMX dalam memecahkan masalah tersebut. Misalnya, bagaimana cara menggunakan SDMX di aplikasi statistik favorit Kamu seperti SAS, R, atau Excel. Bagaimana membuat situs web diseminasi maupun membangun sistem pengumpulan data yang tangguh.

Dan terakhir, perhatikan Model Informasi SDMX dan pahami bagaimana model tersebut dapat mendukung *use cases* yang Kamu miliki. Ketika Kamu mempelajari model ini (kami akan menjelaskan model ini nanti) kami yakin bahwa Kamu akan menyadari bahwa SDMX dapat memenuhi kebutuhan-kebutuhanmu. Kemudian dengan aplikasi *open source*, Kamu juga akan mendapati bahwa mengimplementasinya pada sistemmu akan jauh lebih cepat dari apa yang Kamu bayangkan sebelumnya.

Model yang sudah Matang
-----------------------

SDMX, pada intinya, adalah Model Informasi yang diimplementasikan dalam sintaks tertentu (terutama XML). SDMX responsif terhadap teknologi baru karena representasi sintaksis dapat dibangun dengan mudah serta memiliki basis Model Informasi. Sebagai contoh, format JSON terbaru telah dikembangkan dan format tersebut semakin populer di kalangan pengembang web.

Kami telah menerapkan sistem pengumpulan data, validasi data, dan diseminasi data untuk sejumlah klien. Kami juga telah membangun aplikasi SDMX sejak tahun 2005, dan kami telah mengembangkan dan merilis SdmxSource (*open source*). Kami senang untuk berbagi pengetahuan ini untuk menunjukkan bagaimana sistem dengan "SDMX Inside" dapat memungkinkan Kamu untuk menemukan solusi dengan biaya yang sedikit, sumber daya yang sedikit baik pada tahap inisiasi maupun pada tahap yang sedang berlangsung, serta dalam waktu yang lebih singkat.

Model Informasi adalah sintaks dengan format agnostik [#f1]_ yang sebagian besar proses dan fungsi dapat dikembangkan di sekitar model, dan bukan di sekitar sintaks. Ini adalah inti dari *SDMX Source* (www.sdmxsource.org) yang terdiri dari aplikasi *open source* yang digunakan untuk mengembangkan aplikasi berbasis SDMX. Banyak aplikasi telah dikembangkan untuk memproses SDMX (*reading*, *writing*, validasi, transformasi, pemetaan). Aplikasi-aplikasi tersebut dapat digabung dan dijadikan satu ke dalam sistem tanpa menghiraukan pembuat dari suatu komponen tersebut telah memiliki pengetahuan untuk mematuhi API yang sama.

*SDMX Source* dikembangkan oleh *Metadata Technology* dan digunakan oleh banyak institusi besar, termasuk Eurostat yang telah mengadopsi *SDMX Source* sebagai *framework* dasar untuk *tools* dan aplikasinya. Pembangunan aplikasi menggunakan *framework* ini dapat menjamin penyesuaian SDMX baik untuk impor maupun ekspor informasi.

Standar ISO
-----------

SDMX hadir dengan sponsor yang berasal dari organisasi internasional (BIS, ECB, Eurostat,IMF, OECD, PBB, Bank Dunia) dan memiliki status ISO (standar internasional 17369). SDMX dijaga dan dipertahankan secara aktif dengan merespons permintaan fungsi baru melalui proses yang terbuka.

Pengembalian Investasi
----------------------

Sering disebutkan, bahwa sulit untuk melakukan justifikasi terhadap investasi pada standar yang spesifik jika hanya digunakan untuk satu hal saja. SDMX dapat melakukan lebih dari sekadar bertindak sebagai format umum untuk bertukar data statistik dan metadata. Jika Kamu menggunakan SDMX sebagai model pada sistem pengumpulan data, *data reporting*, dan diseminasi data, maka akan ada banyak manfaat yang Kamu dapatkan. Semakin banyak Kamu menggunakan kelebihan dari SDMX di sistemmu, semakin banyak manfaat yang akan Kamu peroleh.

.. [#f1] Dalam komputasi, perangkat atau program perangkat lunak dikatakan agnostik atau data agnostik jika metode atau format transmisi data tidak relevan dengan fungsi perangkat atau program. Ini berarti bahwa perangkat atau program dapat menerima data dalam berbagai format atau dari berbagai sumber, dan masih memproses data tersebut secara efektif.
