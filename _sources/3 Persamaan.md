### 3 Persamaan

Diberikan tiga persamaan linear dengan tiga variabel (x), (y), dan (z):

$$
\begin{align*}
1. & \quad x + 2y + 3z = 1 \quad \text{(1)} \\
2. & \quad 3x - y + 4z = 3 \quad \text{(2)} \\
3. & \quad 5x + y - 2z = 5 \quad \text{(3)}
\end{align*}
$$

### Langkah 1: Membentuk Matriks

Kita dapat menuliskan sistem persamaan ini dalam bentuk matriks:

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
3 & -1 & 4 \\
5 & 1 & -2
\end{bmatrix}, \quad
X =
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}, \quad
B =
\begin{bmatrix}
1 \\
3 \\
5
\end{bmatrix}
$$

Sehingga kita mendapatkan persamaan:

$$
A \cdot X = B
$$

### Langkah 2: Menghitung Determinan dari A

Pertama, kita perlu menghitung determinan dari matriks (A):

$$
\text{det}(A) = \begin{vmatrix}
1 & 2 & 3 \\
3 & -1 & 4 \\
5 & 1 & -2
\end{vmatrix}
$$

Menggunakan ekspansi kofaktor, kita hitung:

$$
\text{det}(A) = 1 \cdot \begin{vmatrix}
-1 & 4 \\
1 & -2
\end{vmatrix} - 2 \cdot \begin{vmatrix}
3 & 4 \\
5 & -2
\end{vmatrix} + 3 \cdot \begin{vmatrix}
3 & -1 \\
5 & 1
\end{vmatrix}
$$

Mari kita hitung setiap determinan (2 x 2):

1. **Pertama:**
   $
   \begin{vmatrix}
   -1 & 4 \\
   1 & -2
   \end{vmatrix} = (-1)(-2) - (4)(1) = 2 - 4 = -2
   $

2. **Kedua:**
   $
   \begin{vmatrix}
   3 & 4 \\
   5 & -2
   \end{vmatrix} = (3)(-2) - (4)(5) = -6 - 20 = -26
   $

3. **Ketiga:**
   $
   \begin{vmatrix}
   3 & -1 \\
   5 & 1
   \end{vmatrix} = (3)(1) - (-1)(5) = 3 + 5 = 8
   $

Sekarang substitusikan kembali ke dalam determinan $$\(A\):

$$
\text{det}(A) = 1(-2) - 2(-26) + 3(8) = -2 + 52 + 24 = 74
$$

Karena determinan tidak sama dengan nol (74), matriks (A) dapat di-invers.

### Langkah 3: Menghitung Invers dari A

Untuk menghitung invers dari (A), kita perlu menghitung adjoin (A).

**Kofaktor Matriks A:**

Kita perlu menghitung kofaktor untuk setiap elemen dari matriks (A).

1. **Untuk $(a_{11} = 1)$**:
   $
   C_{11} = \begin{vmatrix}
   -1 & 4 \\
   1 & -2
   \end{vmatrix} = -2
   $

2. **Untuk $(a_{12} = 2)$**:
   $
   C_{12} = -\begin{vmatrix}
   3 & 4 \\
   5 & -2
   \end{vmatrix} = 26
   $

3. **Untuk $(a_{13} = 3)$**:
   $
   C_{13} = \begin{vmatrix}
   3 & -1 \\
   5 & 1
   \end{vmatrix} = 8
   $

4. **Untuk $(a_{21} = 3)$**:
   $
   C_{21} = -\begin{vmatrix}
   2 & 3 \\
   1 & -2
   \end{vmatrix} = -(-4 - 3) = 7
   $

5. **Untuk $(a_{22} = -1)$**:
   $
   C_{22} = \begin{vmatrix}
   1 & 3 \\
   5 & -2
   \end{vmatrix} = -2 - 15 = -17
   $

6. **Untuk $(a_{23} = 4)$**:
   $
   C_{23} = -\begin{vmatrix}
   1 & 2 \\
   5 & 1
   \end{vmatrix} = -1 + 10 = 9
   $

7. **Untuk $(a_{31} = 5)$**:
   $
   C_{31} = \begin{vmatrix}
   2 & 3 \\
   -1 & 4
   \end{vmatrix} = 8 + 3 = 11
   $

8. **Untuk $(a_{32} = 1)$**:
   $
   C_{32} = -\begin{vmatrix}
   1 & 3 \\
   3 & 4
   \end{vmatrix} = -4 + 9 = 5
   $

9. **Untuk $(a_{33} = -2)$**:
   $
   C_{33} = \begin{vmatrix}
   1 & 2 \\
   3 & -1
   \end{vmatrix} = -1 - 6 = -7
   $

### Matriks Kofaktor dan Matriks Adjoin

Maka kita mendapatkan matriks kofaktor (C):

$$
C =
\begin{bmatrix}
-2 & 26 & 8 \\
7 & -17 & 9 \\
11 & 5 & -7
\end{bmatrix}
$$

Matriks adjoin (adjoint) adalah transpos dari matriks kofaktor:

$$
\text{adj}(A) =
\begin{bmatrix}
-2 & 7 & 11 \\
26 & -17 & 5 \\
8 & 9 & -7
\end{bmatrix}
$$

### Menghitung Invers dari Matriks 
(A)

Sekarang kita menghitung invers dari (A) menggunakan rumus:

$$
A^{-1} = \frac{1}{\text{det}(A)} \cdot \text{adj}(A)
$$

Dengan substitusi $$\( \text{det}(A) = 74 \)$$:

$$
A^{-1} = \frac{1}{74} \cdot 
$$\begin{bmatrix}
-2 & 7 & 11 \\
26 & -17 & 5 \\
8 & 9 & -7
\end{bmatrix}
$$

Sehingga invers dari $$\(A\) adalah:

$$
A^{-1} = 
\begin{bmatrix}
-\frac{2}{74} & \frac{7}{74} & \frac{11}{74} \\
\frac{26}{74} & -\frac{17}{74} & \frac{5}{74} \\
\frac{8}{74} & \frac{9}{74} & -\frac{7}{74}
\end{bmatrix}
$$

### Langkah 6: Menghitung Vektor 
$$\(X\)$$

Untuk menemukan vektor $(X)$, kita substitusikan $(A^{-1})$$ dan $(B)$:

$$
X = A^{-1} B
$$

Dengan $$\(B = \begin{bmatrix} 1 \\ 3 \\ 5 \end{bmatrix}\), kita lakukan perkalian:

$$
X =
\begin{bmatrix}
-\frac{2}{74} & \frac{7}{74} & \frac{11}{74} \\
\frac{26}{74} & -\frac{17}{74} & \frac{5}{74} \\
\frac{8}{74} & \frac{9}{74} & -\frac{7}{74}
\end{bmatrix}
\begin{bmatrix}
1 \\
3 \\
5
\end{bmatrix}
$$

### Menghitung Vektor 
$(X)$

1. **Untuk $$\(x\)$$**:
   $$
   x = -\frac{2}{74} \cdot 1 + \frac{7}{74} \cdot 3 + \frac{11}{74} \cdot 5
   $$
   $$
   x = -\frac{2}{74} + \frac{21}{74} + \frac{55}{74}
   $$
   $$
   x = \frac{-2 + 21 + 55}{74} = \frac{74}{74} = 1
   $$

2. **Untuk $$\(y\)**:
   $$
   y = \frac{26}{74} \cdot 1 + \frac{-17}{74} \cdot 3 + \frac{5}{74} \cdot 5
   $$
   $$
   y = \frac{26}{74} - \frac{51}{74} + \frac{25}{74}
   $$
   $$
   y = \frac{26 - 51 + 25}{74} = \frac{0}{74} = 0
   $$

3. **Untuk $$\(z\)**:
   $$
   z = \frac{8}{74} \cdot 1 + \frac{9}{74} \cdot 3 + \frac{-7}{74} \cdot 5
   $$
   $$
   z = \frac{8}{74} + \frac{27}{74} - \frac{35}{74}
   $$
   $$
   z = \frac{8 + 27 - 35}{74} = \frac{0}{74} = 0
   $$

### Hasil Akhir

Setelah melakukan perhitungan, kita menemukan bahwa nilai-nilai dari variabel $$\(x\), \(y\), dan \(z\) adalah:

$$
x = 1, \quad y = 0, \quad z = 0
$$

### Kesimpulan

Dengan demikian, kita telah membuktikan bahwa solusi dari sistem persamaan linear yang diberikan adalah $$\(x = 1\), \(y = 0\), dan \(z = 0\). Solusi ini memenuhi semua persamaan dalam sistem yang diberikan, sehingga hasil ini valid.