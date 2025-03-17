# Welcome to Komputasi Aljabar Linier

Komputasi aljabar linier adalah cabang matematika yang mempelajari vektor, matriks, dan sistem persamaan linier, serta transformasi linier yang menghubungkan objek-objek tersebut. Dalam konteks komputasi, aljabar linier digunakan untuk menyelesaikan berbagai masalah di bidang ilmu komputer, statistik, fisika, dan teknik, seperti dalam algoritma machine learning, grafika komputer, dan optimasi. Konsep kunci dalam aljabar linier meliputi vektor, matriks, ruang vektor, serta eigenvalue dan eigenvector, yang semuanya berperan penting dalam analisis data dan pemodelan matematis.

# Sistem Persamaan Linier
Sistem persamaan linier adalah sekumpulan dua atau lebih persamaan linier yang memiliki dua atau lebih variabel. Tujuan dari sistem ini adalah untuk menemukan nilai variabel-variabel tersebut yang memenuhi semua persamaan dalam sistem.

## Solusi Sistem Persamaan Linier
Solusi dari sistem persamaan linier adalah nilai-nilai variabel yang memenuhi semua persamaan dalam sistem tersebut. Tergantung pada sifat sistem, solusi bisa berupa satu solusi unik, di mana terdapat satu set nilai yang memenuhi semua persamaan. Ini terjadi ketika garis-garis yang merepresentasikan persamaan berpotongan di satu titik. Namun, sistem juga bisa tidak memiliki solusi sama sekali, yaitu ketika persamaan yang ada saling bertentangan dan garis-garis tersebut sejajar. Selain itu, ada pula kemungkinan bahwa sistem memiliki solusi tak terhingga, yang terjadi ketika semua persamaan dalam sistem adalah kelipatan satu sama lain. Untuk menemukan solusi, berbagai metode dapat digunakan, seperti substitusi, eliminasi, metode matriks, atau grafik, yang semuanya akan memberikan hasil yang sama, yaitu nilai-nilai variabel yang merupakan solusi dari sistem tersebut.

### 1. Satu Solusi
#### Contoh Sistem Persamaan

\[
\begin{align*}
x + 2y + 3z &= 9 \\
2x + 3y + z &= 8 \\
3x + y + 2z &= 7
\end{align*}
\]

<iframe src="https://www.geogebra.org/3d/nm5kbzvu?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**: 
   
[1 2 3 | 9]
[2 3 1 | 8]
[3 1 2 | 7]
   

2. **Eliminasi**:
- Ubah baris 2 dan 3:
R2 = R2 - 2R1
R3 = R3 - 3R1
Hasil menjadi:
[1 2 3 | 9]
[0 -1 -5 | -10]
[0 -5 -7 | -20]
   

- Ubah baris 3:
R3 = R3 - 5R2
Hasil menjadi:
[1 2 3 | 9]
[0 -1 -5 | -10]
[0 0 0 | 0]
   

3. **Back Substitution**:
- Dari baris 2: y + 5z = 10 → y = 10 - 5z
-Dari baris 1: x + 2(10 - 5z) + 3z = 9

   Solusi unik diperoleh dengan nilai tertentu.

### 2. Solusi Tak Hingga

#### Contoh Sistem Persamaan

x + 2y + z = 5
2x + 4y + 2z = 10
3x + 6y + 3z = 15

<iframe src="https://www.geogebra.org/3d/kqxxdwne?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**:
   
[1 2 1 | 5]
[2 4 2 | 10]
[3 6 3 | 15]
   
2. **Eliminasi**:
- Ubah baris 2 dan 3:
R2 = R2 - 2R1
R3 = R3 - 3R1
Hasil menjadi:
[1 2 1 | 5]
[0 0 0 | 0]
[0 0 0 | 0]

### 3. Tanpa Solusi

#### Contoh Sistem Persamaan

x + y + z = 2
2x + 2y + 2z = 3
3x + 3y + 3z = 5

<iframe src="https://www.geogebra.org/3d/n6x44qtc?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**:
   
[1 1 1 | 2]
[2 2 2 | 3]
[3 3 3 | 5]
   
2. **Eliminasi**:
- Ubah baris 2 dan 3:
R2 = R2 - 2R1
R3 = R3 - 3R1
Hasil menjadi:
[1 1 1 | 2]
[0 0 0 | -1]
[0 0 0 | -1]