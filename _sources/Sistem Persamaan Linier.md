# Contoh Persamaan Linier

### 1. Satu Solusi
#### Contoh Sistem Persamaan

$$\begin{align*}
x + 2y + 3z &= 9 \\
2x + 3y + z &= 8 \\
3x + y + 2z &= 7
\end{align*}$$

<iframe src="https://www.geogebra.org/3d/nm5kbzvu?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**: 

$$\begin{align*} 
[1 2 3 | 9] \\
[2 3 1 | 8] \\
[3 1 2 | 7]
\end{align*}$$

2. **Eliminasi**:
- Ubah baris 2 dan 3:

$$\begin{align*}
R2 = R2 - 2R1 <br>
R3 = R3 - 3R1
Hasil menjadi:

$$\begin{align*}
[1  2  3 | 9] \\
[0 -1 -5 | -10] \\
[0 -5 -7 | -20]
\end{align*}$$

- Ubah baris 3:
R3 = R3 - 5R2
Hasil menjadi:

$$\begin{align*}
[1 2 3 | 9] \\
[0 -1 -5 | -10] \\
[0 0 0 | 0]
\end{align*}$$

3. **Back Substitution**:
- Dari baris 2: y + 5z = 10 → y = 10 - 5z <br>
-Dari baris 1: x + 2(10 - 5z) + 3z = 9

   Solusi unik diperoleh dengan nilai tertentu.

### 2. Solusi Tak Hingga

#### Contoh Sistem Persamaan

$$\begin{align*}
x + 2y + z = 5 \\
2x + 4y + 2z = 10 \\
3x + 6y + 3z = 15
\end{align*}$$

<iframe src="https://www.geogebra.org/3d/kqxxdwne?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**:
   
$$\begin{align*}
[1 2 1 | 5] \\
[2 4 2 | 10] \\
[3 6 3 | 15]
\end{align*}$$
   
2. **Eliminasi**:
- Ubah baris 2 dan 3:
R2 = R2 - 2R1
R3 = R3 - 3R1
Hasil menjadi:

$$\begin{align*}
[1 2 1 | 5] \\
[0 0 0 | 0] \\
[0 0 0 | 0]
\end{align*}$$

### 3. Tanpa Solusi

#### Contoh Sistem Persamaan

$$\begin{align*}
x + y + z = 2 \\
2x + 2y + 2z = 3 \\
3x + 3y + 3z = 5
\end{align*}$$

<iframe src="https://www.geogebra.org/3d/n6x44qtc?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

#### Langkah Penyelesaian:
1. **Matriks Augmented**:
   
$$\begin{align*}
[1 1 1 | 2] \\
[2 2 2 | 3] \\
[3 3 3 | 5]
\end{align*}$$

2. **Eliminasi**:
- Ubah baris 2 dan 3:
R2 = R2 - 2R1
R3 = R3 - 3R1
Hasil menjadi:

$$\begin{align*}
[1 1 1 | 2] \\
[0 0 0 | -1] \\
[0 0 0 | -1]
\end{align*}$$