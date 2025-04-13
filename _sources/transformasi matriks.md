## Matrix Transformations
 Tujuan kita adalah untuk mendapatkan pemahaman visual tentang definisi perkalian matriks kita akan melihat bahwa definisi ini memungkinkan kita menggunakan matriks untuk mendefinisikan fungsi yang mengubah satu vektor menjadi vektor lainnya. 

Diberikan matriks A berukuran m×n, kita dapat mendefinisikan fungsi T yang mengambil vektor kolom n×1 ⃗x ∈ Rn sebagai input, dan menghasilkan vektor kolom m×1 ⃗y ∈ Rm sebagai output, sesuai dengan hubungan
 ⃗⃗y = T(⃗x) = A⃗x. 
Fungsi ini dikenal sebagai transformasi matriks, dan merupakan contoh dari klasifikasi fungsi yang lebih umum antara ruang vektor yang disebut transformasi linear. Representasi grafis vektor memungkinkan kita untuk memvisualisasikan transformasi matriks, yang berperan penting dalam aplikasi seperti grafik komputer. 

Untuk menyederhanakan diskusi, kita akan fokus pada vektor dalam R2. Kita ingin memvisualisasikan hasil penggandaan vektor dengan matriks. Agar bisa mengalikan vektor 2D dengan matriks dan mendapatkan vektor 2D kembali, matriks kita harus berupa matriks kuadrat berukuran 2 × 2. Kita akan memulai dengan contoh. Diberikan matriks A dan beberapa vektor, kita akan menggambar vektor sebelum dan setelah dikalikan dengan A 

Mengalikan vektor dengan matriks. Misalkan A adalah matriks, dan ⃗x, ⃗y, dan ⃗z adalah vektor seperti yang diberikan di bawah ini. 
$[
A = \begin{bmatrix}
1 & 4 \\
2 & 3
\end{bmatrix}, \quad
\mathbf{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}, \quad
\mathbf{y} = \begin{bmatrix}
-1 \\
1
\end{bmatrix}, \quad
\mathbf{z} = \begin{bmatrix}
3 \\
-1
\end{bmatrix}.
]$

Graph ⃗x, ⃗y and ⃗z, as well as A⃗x, A⃗y and A⃗z.

Solution. It is straightforward to compute:
$[
A\vec{x} = \begin{bmatrix}
5 \\
5
\end{bmatrix}, 
A\vec{y} = \begin{bmatrix}
3 \\
1
\end{bmatrix}, 
\text{and } A\vec{z} = \begin{bmatrix}
-1 \\
3
\end{bmatrix}.
]$

The vectors are sketched in Figure 5.1.2.
(path/to/figure5.1.2.png)

Ada beberapa hal yang perlu diperhatikan. Ketika setiap vektor dikalikan dengan A, hasilnya adalah vektor dengan panjang yang berbeda (dalam contoh ini, selalu lebih panjang), dan dalam dua kasus (untuk ⃗y dan \vz), vektor yang dihasilkan mengarah ke arah yang berbeda. Ini tidak mengejutkan. Pada bagian sebelumnya, kita belajar tentang perkalian matriks, yang merupakan operasi yang aneh dan tampaknya tidak dapat diprediksi. Apakah Anda mengharapkan menemukan pola yang langsung dikenali dari mengalikan matriks dan vektor? (Ini adalah pertanyaan retoris; jawaban yang diharapkan adalah "Tidak. ") Faktanya, hal yang mengejutkan dari contoh ini adalah ⃗x dan A⃗x mengarah ke arah yang sama! Mengapa arah ⃗x tidak berubah setelah dikalikan dengan A? (Kita akan menjawab ini di Bagian 7. 1 saat kita belajar tentang sesuatu yang disebut "vektor eigen. ") 

Matriks yang berbeda bertindak pada vektor dengan cara yang berbeda. (Itu sebabnya kita menyebutnya "berbeda. ") Beberapa selalu meningkatkan panjang vektor melalui perkalian, yang lain selalu mengurangi panjang, beberapa meningkatkan panjang beberapa vektor dan mengurangi panjang yang lain, dan yang lainnya tidak mengubah panjang sama sekali. Pernyataan serupa dapat dibuat tentang bagaimana matriks mempengaruhi arah vektor melalui perkalian: beberapa mengubah arah setiap vektor, beberapa mengubah arah "kebanyakan" vektor tetapi membiarkan beberapa tetap sama, dan yang lainnya masih tidak mengubah arah vektor mana pun. 

Bagaimana kita mempelajari bagaimana perkalian matriks mempengaruhi vektor? Kita bisa saja membuat banyak matriks berbeda dan banyak vektor berbeda, mengalikan, lalu menggambar, tetapi ini akan menjadi pekerjaan yang sangat berat dengan hasil yang sedikit berguna. Akan terlalu sulit menemukan pola perilaku dalam hal ini. (Ingat, itu yang dilakukan matematikawan. Kami mencari pola. ) Sebagai gantinya, kita akan mulai dengan menggunakan teknik yang sering kita gunakan di masa lalu. Kita memiliki operasi "baru"; mari kita eksplorasi bagaimana perilakunya dengan operasi "lama". Secara spesifik, kita tahu cara membuat sketsa penjumlahan vektor. Apa yang terjadi ketika kita memasukkan perkalian matriks ke dalam campuran? Mari kita coba contoh.
Contoh 5.1.3 Menggabungkan penjumlahan dan perkalian matriks.
Misalkan A adalah suatu matriks dan ⃗x dan ⃗y adalah vektor seperti yang diberikan di bawah ini.
$[
A = \begin{bmatrix}
1 & 1 \\
1 & 2 
\end{bmatrix}, \quad 
\mathbf{x} = \begin{bmatrix}
2 \\
1 
\end{bmatrix}, \quad 
\mathbf{y} = \begin{bmatrix}
-1 \\
1 
\end{bmatrix}.
]$
Sketch ⃗x + ⃗y, A⃗x, A⃗y, and A(⃗x + ⃗y).

solusi.
$[
8\mathbf{x} + \mathbf{y} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}; \quad A \mathbf{x} = \begin{bmatrix} 3 \\ 4 \end{bmatrix}; \quad A \mathbf{y} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}, \quad A(\mathbf{x} + \mathbf{y}) = \begin{bmatrix} 3 \\ 5 \end{bmatrix} .
9]$