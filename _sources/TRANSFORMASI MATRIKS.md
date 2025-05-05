---
title: TRANSFORMASI MATRIKS

---

# BAB 5

# MATRIX TRANSFORMATIONS

## 5.1 Matrix Transformations

### 5.1.1 Matrix–Vector Multiplication
- Transformasi matriks adalah fungsi linear dalam bentuk:  
  $T(\vec{x}) = A\vec{x}$
- Matriks $A$ adalah matriks $m \times n$ dan $\vec{x} \in {R}^n$
- Contoh:  
  Jika $A = \begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix}$, dan $\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$, maka:  
  $A\vec{x} = \begin{bmatrix} 5 \\ 5 \end{bmatrix}$

### 5.1.2 Transformations of the Cartesian Plane
- Vektor divisualisasikan sebagai anak panah dari asal ke titik $(x, y)$
- Transformasi matriks memetakan semua vektor, cukup dengan melihat pengaruhnya terhadap unit square:  
  $(0,0), (1,0), (1,1), (0,1)$
- Contoh: $A = \begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix}$ mengubah titik-titik persegi satuan menjadi:  
  $(0,0), (1,2), (5,5), (4,3)$

### 5.1.3 2D Matrix Transformations
- Jenis-jenis transformasi dan matriksnya:

| Transformasi              | Matriks                                       |
|---------------------------|-----------------------------------------------|
| Stretch horizontal        | $\begin{bmatrix} k & 0 \\ 0 & 1 \end{bmatrix}$ |
| Stretch vertikal          | $\begin{bmatrix} 1 & 0 \\ 0 & k \end{bmatrix}$ |
| Shear horizontal          | $\begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}$ |
| Shear vertikal            | $\begin{bmatrix} 1 & 0 \\ k & 1 \end{bmatrix}$ |
| Refleksi sumbu x          | $\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$ |
| Refleksi sumbu y          | $\begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}$ |
| Refleksi terhadap y = x   | $\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$ |
| Rotasi sudut $\theta$      | $\begin{bmatrix} \cos \theta & -\sin \theta \\ \sin \theta & \cos \theta \end{bmatrix}$ |
| Proyeksi ke sumbu x       | $\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}$ |
| Proyeksi ke sumbu y       | $\begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix}$ |

### 5.1.4 Linear Transformations
- Syarat transformasi linear:
  1. $T(\vec{u} + \vec{v}) = T(\vec{u}) + T(\vec{v})$
  2. $T(c \vec{u}) = c T(\vec{u})$
- Transformasi linear mempertahankan sifat penjumlahan dan skalar.
- Secara visual, $A(\vec{u} + \vec{v}) = A\vec{u} + A\vec{v}$ menghasilkan bentuk jajar genjang.

### 5.1.5 Combining Transformations
- Kombinasi beberapa transformasi dapat dilakukan melalui perkalian matriks:
  $$
  A = A_4 A_3 A_2 A_1
  $$
- Urutan perkalian penting karena matriks tidak komutatif: $A_1A_2 \ne A_2A_1$
- Contoh: shear $\rightarrow$ rotasi $\rightarrow$ stretch $\rightarrow$ refleksi, dapat digabungkan menjadi satu matriks komposit.

---
### > Soal Nomor 1
Diketahui:
- $\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$
- $\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$
- $A = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}$

**Jawaban:**
$$
A\vec{x} = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix} \begin{bmatrix} 1 \\ 1 \end{bmatrix} = \begin{bmatrix} 0 \\ 5 \end{bmatrix} \\
A\vec{y} = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix} \begin{bmatrix} -1 \\ 2 \end{bmatrix} = \begin{bmatrix} -3 \\ 4 \end{bmatrix}
$$

### > Soal Nomor 2
Diketahui:
- $A = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}$
- $\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$
- $\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$

**Jawaban:**
$$
A\vec{x} = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix} \begin{bmatrix} 1 \\ 1 \end{bmatrix} = \begin{bmatrix} 2 \\ 2 \end{bmatrix} \\
A\vec{y} = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix} \begin{bmatrix} -1 \\ 2 \end{bmatrix} = \begin{bmatrix} -2 \\ 7 \end{bmatrix}
$$

### > Soal Nomor 5
Soal: Tentukan transformasi matriks berdasarkan gambar (refleksi terhadap garis $y = x$).

**Jawaban:**
$$
A = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

### > Soal Nomor 6
Soal: Tentukan transformasi matriks berdasarkan gambar (refleksi terhadap sumbu-y).

**Jawaban:**
$$
A = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}
$$

---
