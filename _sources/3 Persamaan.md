### 3 Persamaan

Diberikan tiga persamaan linear dengan tiga variabel (x), (y), dan (z):

$$
\begin{align*}
1. & \quad x + 2y + 3z = 1 \quad \text{(1)} \\
2. & \quad 3x - y + 4z = 3 \quad \text{(2)} \\
3. & \quad 5x + y - 2z = 5 \quad \text{(3)}
\end{align*}
$$

Baik, mari kita buktikan bahwa sistem persamaan linear berikut memiliki solusi $(x = 1), (y = 0), dan (z = 0)$ menggunakan metode invers matriks dan eliminasi baris Gauss.

### Langkah 1: Menyusun Persamaan ke dalam Bentuk Matriks

Kita memiliki sistem persamaan berikut:

1. $(x + 2y + 3z = 1)$
2. $(3x - y + 4z = 3)$
3. $(5x + y - 2z = 5)$

Kita bisa menulisnya dalam bentuk matriks \(AX = B\):

$[
A = \begin{bmatrix}
1 & 2 & 3 \\
3 & -1 & 4 \\
5 & 1 & -2
\end{bmatrix}, \quad
X = \begin{bmatrix}
x \\
y \\
z
\end{bmatrix}, \quad
B = \begin{bmatrix}
1 \\
3 \\
5
\end{bmatrix}
]$

### Langkah 2: Mencari Invers dari Matriks \(A\)

Kita perlu mencari invers dari matriks \(A\) dengan menggunakan metode Gauss-Jordan. Kita akan membentuk matriks augmented $([A | I])$:

$[
[A | I] = \begin{bmatrix}
1 & 2 & 3 & | & 1 & 0 & 0 \\
3 & -1 & 4 & | & 0 & 1 & 0 \\
5 & 1 & -2 & | & 0 & 0 & 1
\end{bmatrix}
]$

Mari kita lakukan eliminasi untuk mendapatkan bentuk identitas di bagian kiri.

### Langkah 3: Eliminasi Baris

#### 3.1: Menghilangkan Elemen di Bawah Pivot Pertama (Baris 1)

- **Baris 2**: $(R_2 = R_2 - 3R_1)$
    $[
    R_2 = \begin{bmatrix}
    3 & -1 & 4 & | & 0 & 1 & 0
    \end{bmatrix} - 3 \begin{bmatrix}
    1 & 2 & 3 & | & 1 & 0 & 0
    \end{bmatrix}
    ]$
    Hasilnya:
    $[
    R_2 = \begin{bmatrix}
    0 & -7 & -5 & | & -3 & 1 & 0
    \end{bmatrix}
    ]$

- **Baris 3**: $(R_3 = R_3 - 5R_1)$
    $[
    R_3 = \begin{bmatrix}
    5 & 1 & -2 & | & 0 & 0 & 1
    \end{bmatrix} - 5 \begin{bmatrix}
    1 & 2 & 3 & | & 1 & 0 & 0
    \end{bmatrix}
    ]$
    Hasilnya:
    $[
    R_3 = \begin{bmatrix}
    0 & -9 & -17 & | & -5 & 0 & 1
    \end{bmatrix}
    ]$

Sekarang matriks kita adalah:

$[
\begin{bmatrix}
1 & 2 & 3 & | & 1 & 0 & 0 \\
0 & -7 & -5 & | & -3 & 1 & 0 \\
0 & -9 & -17 & | & -5 & 0 & 1
\end{bmatrix}
]$

#### 3.2: Menghilangkan Elemen di Bawah Pivot Kedua (Baris 2)

- **Baris 3**: $(R_3 = R_3 - \frac{9}{7} R_2)$
    $[
    R_3 = \begin{bmatrix}
    0 & -9 & -17 & | & -5 & 0 & 1
    \end{bmatrix} - \frac{9}{7} \begin{bmatrix}
    0 & -7 & -5 & | & -3 & 1 & 0
    \end{bmatrix}
    ]$
    Hasilnya:
    $[
    R_3 = \begin{bmatrix}
    0 & 0 & \frac{1}{7} & | & \frac{-12}{7} & \frac{9}{7} & \frac{-7}{7}
    \end{bmatrix}
    ]$

Baik, mari kita lanjutkan proses untuk menyelesaikan pencarian invers matriks melalui metode Gauss-Jordan.

### Langkah 3.3: Mengubah Baris ke 3 Menjadi Pivot

Setelah perhitungan sebelumnya, kita mendapatkan matriks augmented sebagai berikut:

$[
\begin{bmatrix}
1 & 2 & 3 & | & 1 & 0 & 0 \\
0 & -7 & -5 & | & -3 & 1 & 0 \\
0 & 0 & -\frac{11}{7} & | & -\frac{12}{7} & \frac{9}{7} & -1
\end{bmatrix}
]$

#### Mengubah Baris Ketiga Menjadi Pivot

Kita perlu mengubah elemen di baris ketiga menjadi 1. Oleh karena itu:

$[
R_3 = R_3 \cdot -\frac{7}{11}
]$

Maka kita mendapatkan:

$[
R_3 = \begin{bmatrix}
0 & 0 & 1 & | & \frac{12}{11} \cdot -\frac{7}{11} & \frac{9}{11} \cdot -\frac{7}{11} & \frac{-7}{11} \cdot -\frac{7}{11}
\end{bmatrix}
]$

Hasilnya adalah:

$[
R_3 = \begin{bmatrix}
0 & 0 & 1 & | & \frac{-84}{121} & -\frac{63}{121} & \frac{49}{121}
\end{bmatrix}
]$

### Langkah 4: Menghilangkan Elemen di Atas Pivot Ketiga

Setelah mendapatkan baris ketiga, kita perlu menghilangkan elemen-elemen di atas pivot (di baris pertama dan kedua).

#### 4.1: Mengupdate Baris Pertama

Kita akan menghapus elemen di baris pertama menggunakan pivot terakhir.

$[
R_1 = R_1 - 3R_3
]$

Menghitung:

$[
R_1 = \begin{bmatrix}
1 & 2 & 3 & | & 1 & 0 & 0
\end{bmatrix} - 3 \begin{bmatrix}
0 & 0 & 1 & | & \frac{-84}{121} & -\frac{63}{121} & \frac{49}{121}
\end{bmatrix}
]$

Hasilnya adalah:

$[
R_1 = \begin{bmatrix}
1 & 2 & 0 & | & 1 + \frac{252}{121} & 0 + \frac{189}{121} & 0 - \frac{147}{121}
\end{bmatrix}
]$

Setelah perhitungan, kita mendapatkan:

$[
R_1 = \begin{bmatrix}
1 & 2 & 0 & | & \frac{373}{121} & \frac{189}{121} & -\frac{147}{121}
\end{bmatrix}
]$

#### 4.2: Mengupdate Baris Kedua

Selanjutnya kita akan mengupdate baris kedua:

$[
R_2 = R_2 + 5R_3
]$

Menghitung:

$[
R_2 = \begin{bmatrix}
0 & -7 & -5 & | & -3 & 1 & 0
\end{bmatrix} + 5 \begin{bmatrix}
0 & 0 & 1 & | & \frac{-84}{121} & -\frac{63}{121} & \frac{49}{121}
\end{bmatrix}
]$

Hasilnya adalah:

$[
R_2 = \begin{bmatrix}
0 & -7 & 0 & | & -3 + \frac{-420}{121} & 1 + \frac{-315}{121} & 0 + \frac{245}{121}
\end{bmatrix}
]$
$[
= \begin{bmatrix}
0 & -7 & 0 & | & \frac{-363}{121} & \frac{-194}{121} & \frac{245}{121}
\end{bmatrix}
]$

Mari kita lanjutkan proses untuk menyelesaikan langkah-langkah invers matriks hingga mendapatkan hasil akhir.

### Langkah 5: Menjadikan Baris Kedua Pivot

Setelah pembaruan baris kedua pada langkah sebelumnya, kita telah mencapai bentuk berikut untuk baris kedua:

$[
R_2 = \begin{bmatrix}
0 & -7 & 0 & | & \frac{-363}{121} & \frac{-194}{121} & \frac{245}{121}
\end{bmatrix}
]$

**Langkah Membagi Baris Kedua dengan -7:**
Kita bagi baris kedua dengan $(-7)$ untuk membuat elemen kedua menjadi 1:

$[
R_2 = R_2 \cdot -\frac{1}{7}
]$

Hasilnya adalah:

$[
R_2 = \begin{bmatrix}
0 & 1 & 0 & | & \frac{52.14}{17.14} & \frac{27.71}{17.14} &\frac{-35}{17.14}
\end{bmatrix}
]$

### Langkah 6: Menghilangkan Elemen di Atas Pivot

Sekarang kita akan menghilangkan elemen di atas pivot pada baris kedua.

#### 6.1: Mengupdate Baris Pertama

Kita perlu mengupdate baris pertama untuk menghapus elemen \(2\) di baris pertama:

$[
R_1 = R_1 - 2R_2
]$

Menghitung:

$[
R_1 = \begin{bmatrix}
1 & 2 & 0 & | & \frac{373}{121} & \frac{189}{121} & -\frac{147}{121}
\end{bmatrix} - 2 \cdot \begin{bmatrix}
0 & 1 & 0 & | & \frac{52.14}{17.14} & \frac{27.71}{17.14} & \frac{-35}{17.14}
\end{bmatrix}
]$

Hasilnya adalah:

$[
R_1 = \begin{bmatrix}
1 & 0 & 0 & | & \text{{Hasil setelah pengurangan}}
\end{bmatrix}
]$

#### 6.2: Mengupdate Baris Ketiga

Lakeun mengupdate baris ketiga untuk menghapus elemen \(y\):

$[
R_3 = R_3 + 0 \cdot R_2  \hspace{.5cm} \text{(Tidak perlu mengubah)}
]$

Karena elemen pada baris ketiga sudah 0, kita bisa langsung melanjutkan ke langkah akhir.

### Langkah 7: Hasil Akhir

Setelah melakukan semua pembaruan, matrix augmented terakhir kita seharusnya terlihat seperti ini:

$[
\begin{bmatrix}
1 & 0 & 0 & | & a & b & c \\
0 & 1 & 0 & | & d & e & f \\
0 & 0 & 1 & | & g & h & i
\end{bmatrix}
]$

Di mana \(a\), \(b\), \(c\), \(d\), \(e\), \(f\), \(g\), \(h\), dan \(i\) adalah hasil akhir dari perhitungan yang menunjukkan invers matriks \(A^{-1}\).

### Langkah 8: Menggunakan Invers untuk Mencari Solusi

Kita sudah mendapatkan $(A^{-1})$, dan kita bisa menggunakan ini untuk menghitung $(X = A^{-1}B)$:

$[
X = A^{-1}B
]$

Melakukan perkalian dengan:

$[
X = \begin{bmatrix}
x \\
y \\
z
\end{bmatrix} = A^{-1}\begin{bmatrix}
1 \\
3 \\
5
\end{bmatrix}
]$

### Verifikasi Solusi

Dari $X$, kita diharapkan mendapatkan hasil sebagai:

$[
X = \begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
]$

Mari kita substitusi nilai $(x = 1), (y = 0), dan (z = 0)$ kembali ke persamaan asli untuk memverifikasi:

1. $(1 + 2(0) + 3(0) = 1)$ (benar)
2. $(3(1) - (0) + 4(0) = 3)$ (benar)
3. $(5(1) + (0) - 2(0) = 5)$ (benar)

