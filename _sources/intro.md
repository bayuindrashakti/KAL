# Welcome to Komputasi Aljabar Linier

Komputasi aljabar linier adalah cabang matematika yang mempelajari vektor, matriks, dan sistem persamaan linier, serta transformasi linier yang menghubungkan objek-objek tersebut. Dalam konteks komputasi, aljabar linier digunakan untuk menyelesaikan berbagai masalah di bidang ilmu komputer, statistik, fisika, dan teknik, seperti dalam algoritma machine learning, grafika komputer, dan optimasi. Konsep kunci dalam aljabar linier meliputi vektor, matriks, ruang vektor, serta eigenvalue dan eigenvector, yang semuanya berperan penting dalam analisis data dan pemodelan matematis.

# Sistem Persamaan Linier
Sistem persamaan linier adalah sekumpulan dua atau lebih persamaan linier yang memiliki dua atau lebih variabel. Tujuan dari sistem ini adalah untuk menemukan nilai variabel-variabel tersebut yang memenuhi semua persamaan dalam sistem.

## Solusi Sistem Persamaan Linier
Solusi dari sistem persamaan linier adalah nilai-nilai variabel yang memenuhi semua persamaan dalam sistem tersebut. Tergantung pada sifat sistem, solusi bisa berupa satu solusi unik, di mana terdapat satu set nilai yang memenuhi semua persamaan. Ini terjadi ketika garis-garis yang merepresentasikan persamaan berpotongan di satu titik. Namun, sistem juga bisa tidak memiliki solusi sama sekali, yaitu ketika persamaan yang ada saling bertentangan dan garis-garis tersebut sejajar. Selain itu, ada pula kemungkinan bahwa sistem memiliki solusi tak terhingga, yang terjadi ketika semua persamaan dalam sistem adalah kelipatan satu sama lain. Untuk menemukan solusi, berbagai metode dapat digunakan, seperti substitusi, eliminasi, metode matriks, atau grafik, yang semuanya akan memberikan hasil yang sama, yaitu nilai-nilai variabel yang merupakan solusi dari sistem tersebut.

### 1. Satu Solusi
#### Contoh Sistem Persamaan

\begin{align*}
x + 2y + 3z &= 9 \quad (1) \\
2x + 3y + z &= 8 \quad (2) \\
3x + y + 2z &= 7 \quad (3)
\end{align*}

<iframe src="https://www.geogebra.org/3d/nm5kbzvu?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**: 
   
   \begin{bmatrix}
   1 & 2 & 3 & | & 9 \\
   2 & 3 & 1 & | & 8 \\
   3 & 1 & 2 & | & 7
   \end{bmatrix}
   

2. **Eliminasi**:
   - Ubah baris 2 dan 3:
  
   R_2 <- R_2 - 2R_1 ... R_3 <- R_3 - 3R_1
   
   Hasil menjadi:
   
   \begin{bmatrix}
   1 & 2 & 3 & | & 9 \\
   0 & -1 & -5 & | & -10 \\
   0 & -5 & -7 & | & -20
   \end{bmatrix}
   

   - Ubah baris 3:
   
   R_3 <- R_3 - 5R_2
  
   Hasil menjadi:
   
   \begin{bmatrix}
   1 & 2 & 3 & | & 9 \\
   0 & -1 & -5 & | & -10 \\
   0 & 0 & 0 & | & 0
   \end{bmatrix}
   

3. **Back Substitution**:
   - Dari baris 2: \(y + 5z = 10 -> y = 10 - 5z\)
   - Dari baris 1: \(x + 2(10 - 5z) + 3z = 9\)

   Solusi unik diperoleh dengan nilai tertentu.

### 2. Solusi Tak Hingga

#### Contoh Sistem Persamaan

\begin{align*}
x + 2y + z &= 5 \quad (1) \\
2x + 4y + 2z &= 10 \quad (2) \\
3x + 6y + 3z &= 15 \quad (3)
\end{align*}

<iframe src="https://www.geogebra.org/3d/kqxxdwne?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**:
   
   \begin{bmatrix}
   1 & 2 & 1 & | & 5 \\
   2 & 4 & 2 & | & 10 \\
   3 & 6 & 3 & | & 15
   \end{bmatrix}
   

2. **Eliminasi**:
   - Ubah baris 2 dan 3:
   
   R_2 <- R_2 - 2R_1 ... R_3 <- R_3 - 3R_1
   
   Hasil menjadi:
   
   \begin{bmatrix}
   1 & 2 & 1 & | & 5 \\
   0 & 0 & 0 & | & 0 \\
   0 & 0 & 0 & | & 0
   \end{bmatrix}

### 3. Tanpa Solusi

#### Contoh Sistem Persamaan

\begin{align*}
x + y + z &= 2 \quad (1) \\
2x + 2y + 2z &= 3 \quad (2) \\
3x + 3y + 3z &= 5 \quad (3)
\end{align*}

<iframe src="https://www.geogebra.org/3d/n6x44qtc?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**:
   
   \begin{bmatrix}
   1 & 1 & 1 & | & 2 \\
   2 & 2 & 2 & | & 3 \\
   3 & 3 & 3 & | & 5
   \end{bmatrix}
   

2. **Eliminasi**:
   - Ubah baris 2 dan 3:
   
   R_2 <- R_2 - 2R_1 ... R_3 <- R_3 - 3R_1
   
   Hasil menjadi:
   
   \begin{bmatrix}
   1 & 1 & 1 & | & 2 \\
   0 & 0 & 0 & | & -1 \\
   0 & 0 & 0 & | & -1
   \end{bmatrix}