### 3 Persamaan

Diberikan tiga persamaan linear dengan tiga variabel (x), (y), dan (z):

$$
\begin{align*}
1. & \quad x + 2y + 3z = 1 \quad \text{(1)} \\
2. & \quad 3x - y + 4z = 3 \quad \text{(2)} \\
3. & \quad 5x + y - 2z = 5 \quad \text{(3)}
\end{align*}
$$

Baik, mari kita detailkan langkah-langkah penyelesaian sistem persamaan linear $\(x + 2y + 3z = 1\), \(3x - y + 4z = 3\), dan \(5x + y - 2z = 5\)$ menggunakan metode invers matriks dan eliminasi Gauss.

### Langkah 1: Menyusun Matriks Augmented
Kita mulai dengan menuliskan sistem persamaan dalam bentuk matriks. Matriks koefisien untuk sistem ini adalah:

$$\[
A = \begin{bmatrix}
1 & 2 & 3 \\
3 & -1 & 4 \\
5 & 1 & -2
\end{bmatrix}
\]$$

Dan matriks konstanta (hasil dari persamaan) adalah:

$$\[
B = \begin{bmatrix}
1 \\
3 \\
5
\end{bmatrix}
\]$$

Sehingga kita dapat menyusun matriks augmented $\( [A | B] \)$:

$$\[
\begin{bmatrix}
1 & 2 & 3 & | & 1 \\
3 & -1 & 4 & | & 3 \\
5 & 1 & -2 & | & 5
\end{bmatrix}
\]$$

### Langkah 2: Menggunakan Eliminasi Gauss
Kita akan melakukan operasi baris elementer untuk mengubah matriks menjadi bentuk eselon.

#### Langkah 2.1: Menghilangkan Elemen di Bawah Pivot Pertama
Kita akan menghilangkan $\(3\) dan \(5\)$ di bawah elemen pertama (pivot $\(1\)$).

- **Mengupdate baris kedua**:
$$\[
R_2 = R_2 - 3R_1 \rightarrow [3, -1, 4 | 3] - 3 \times [1, 2, 3 | 1] 
\]$$
$$\[
R_2 = [3 - 3, -1 - 6, 4 - 9 | 3 - 3] = [0, -7, -5 | 0]
\]$$

- **Mengupdate baris ketiga**:
$$\[
R_3 = R_3 - 5R_1 \rightarrow [5, 1, -2 | 5] - 5 \times [1, 2, 3 | 1]
\]$$
$$\[
R_3 = [5 - 5, 1 - 10, -2 - 15 | 5 - 5] = [0, -9, -17 | 0]
\]$$

Setelah eliminasi, matriksnya menjadi:

$$\[
\begin{bmatrix}
1 & 2 & 3 & | & 1 \\
0 & -7 & -5 & | & 0 \\
0 & -9 & -17 & | & 0
\end{bmatrix}
\]$$

#### Langkah 2.2: Menghilangkan Elemen di Bawah Pivot Kedua
Sekarang kita akan menghilangkan elemen di bawah $\( -7 \) untuk mendapatkan \(0\)$ pada baris ketiga:

- **Mengupdate baris ketiga**:
$$\[
R_3 = R_3 - \frac{9}{7}R_2 
\]$$
$$\[
R_3 = [0, -9, -17 | 0] - \frac{9}{7} \times [0, -7, -5 | 0]
\]$$
$$\[
R_3 = [0, -9 + 9, -17 + \frac{45}{7} | 0 - 0] = [0, 0, -\frac{11}{7} | 0]
\]$$

Setelah eliminasi, matriksnya menjadi:

$$\[
\begin{bmatrix}
1 & 2 & 3 & | & 1 \\
0 & -7 & -5 & | & 0 \\
0 & 0 & -\frac{11}{7} & | & 0
\end{bmatrix}
\]$$

### Langkah 3: Penyelesaian
Sekarang kita memiliki sistem yang lebih sederhana:
$$
1. \( x + 2y + 3z = 1 \)
2. \( -7y - 5z = 0 \)
3. \( -\frac{11}{7} z = 0 \)
$$

Dari persamaan ketiga, kita dapat langsung menyimpulkan:
$\[
z = 0
\]$

Menggantikan nilai $\(z\)$ ke dalam persamaan kedua:
$\[
-7y - 5(0) = 0 \quad \Rightarrow \quad -7y = 0 \quad \Rightarrow \quad y = 0
\]$

Baik, mari kita lanjutkan dengan proses penyelesaian dari langkah sebelumnya tanpa menggunakan determinan. Kita sudah memperoleh nilai $\(z = 0\) dan \(y = 0\)$. Mari kita substitusikan kembali nilai-nilai ini ke dalam persamaan pertama.

### Langkah 4: Substitusi untuk Mencari nilai \(x\)

Dari persamaan pertama:
$\[
x + 2y + 3z = 1
\]$
Dengan substitusi $\(y = 0\) dan \(z = 0\)$:
$$\[
x + 2(0) + 3(0) = 1
\]
\[
x = 1
\]$$

### Penyelesaian Akhir
Kita telah menemukan bahwa solusi untuk sistem persamaan linear tersebut adalah:
$$\[
x = 1, \quad y = 0, \quad z = 0
\]
$$
