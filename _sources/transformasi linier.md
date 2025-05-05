# Transformasi Linier

---

## Pengantar Transformasi Linier

- **Definisi:** Transformasi linier adalah fungsi yang memetakan ruang vektor *V* ke ruang vektor *W*, dinyatakan sebagai T: V → W. Fungsi ini mengubah vektor dari satu ruang ke ruang lainnya dengan mempertahankan struktur aljabar.
  
- **Contoh Fungsi:** Fungsi dari R² ke R² yang didefinisikan sebagai T(v₁, v₂) = (v₁ + v₂, v₁ - v₂).
  
- **Operasi:**
  - *Mencari Bayangan:* Contoh: Untuk v = (-1, 2), bayangan T(v) dihitung dengan substitusi ke dalam fungsi T.
  - *Mencari Prabayangan:* Contoh: Untuk w = (-1, 11), prabayangan vektor yang dipetakan ke w dicari dengan menyelesaikan persamaan T(v) = w.

---

## Sifat Transformasi Linier

- **Sifat Utama:**
  - *Penjumlahan:* T(v + u) = T(v) + T(u) untuk semua v, u ∈ V.
  - *Perkalian Skalar:* T(cu) = cT(u) untuk semua vektor *u* dan skalar *c*.

- **Catatan:** Transformasi linier disebut juga operator linear yang mempertahankan struktur aljabar.

---

## Verifikasi Transformasi Linier

Verifikasi dilakukan dengan membuktikan sifat penjumlahan dan perkalian skalar untuk fungsi yang dimaksud.

---

## Contoh Fungsi yang Bukan Transformasi Linier

- f(x) = sin(x), tidak memenuhi sifat penjumlahan.
- f(x) = x², tidak memenuhi sifat perkalian skalar.

---

## Jenis Transformasi Linier

- *Transformasi Nol:* Memetakan semua vektor ke nol: T(v) = 0.
- *Transformasi Identitas:* Memetakan setiap vektor ke dirinya sendiri: T(v) = v.

---

## Matriks untuk Transformasi Linier

Transformasi linier dapat dinyatakan dengan matriks *A*, sehingga T(v) = Av.

---

## Rotasi dan Proyeksi

- *Rotasi dalam R²:* Dinyatakan dengan matriks rotasi:  
  A = [cos(θ) -sin(θ); sin(θ) cos(θ)].
  
- *Proyeksi dalam R³:* Dinyatakan dengan matriks proyeksi:  
  A = 
  $$\begin{align*}
    [0 0 0]\\
    [0 1 0]
    [0 0 1]
    \end{align*}$$

---

## Invers Transformasi Linier

Transformasi linier memiliki invers T⁻¹ jika T(T⁻¹(v)) = v untuk semua v ∈ V.

---

## Matriks Relatif dan Perbandingan Matriks

Menemukan matriks relatif terhadap basis nonstandar dan membandingkan dua matriks transformasi.

---

## Catatan tentang Matriks Diagonal

Matriks diagonal adalah matriks dengan elemen non-nol hanya pada diagonal utama dan banyak digunakan dalam transformasi linier.

---

## TUGAS

Transformasi:  
T(v₁, v₂) = (v₁ + v₂, v₁)

### Langkah Membuktikan Transformasi Linier:

#### Definisi Transformasi Linier:

Transformasi T dikatakan linier jika memenuhi dua sifat:
- Homogenitas: T(c * v) = c * T(v) untuk setiap skalar c dan vektor v.
- Superposisi: T(v + w) = T(v) + T(w) untuk setiap vektor v dan w.

#### Buktikan Homogenitas:

Ambil v = (v₁, v₂) dan skalar c:  
T(c * (v₁, v₂)) = T(c * v₁, c * v₂) = (c * v₁ + c * v₂, c * v₁)  
Menjadi: = c * (v₁ + v₂, v₁) = c * T(v)

#### Buktikan Superposisi:

Ambil v = (v₁, v₂) dan w = (w₁, w₂):  
T(v + w) = T(v₁ + w₁, v₂ + w₂) = ((v₁ + w₁) + (v₂ + w₂), v₁ + w₁)  
Menjadi: = (v₁ + v₂ + w₁ + w₂, v₁ + w₁) = (v₁ + v₂, v₁) + (w₁ + w₂, w₁) = T(v) + T(w)

---

## Kesimpulan:

Karena T memenuhi kedua sifat, maka T(v₁, v₂) = (v₁ + v₂, v₁) adalah transformasi linier.

---

## Refleksi ke Sumbu X
Refleksi ke sumbu X dapat dinyatakan dengan transformasi linier yang memetakan setiap titik (x, y) ke (x, -y). Matriks yang merepresentasikan refleksi ini adalah:

$$
A = \begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
$$

### Contoh 1:

Jika kita memiliki titik P(3, 4), maka refleksi P ke sumbu X adalah:

$$
P' = A \cdot P = \begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix} \cdot \begin{bmatrix}
3 \\
4
\end{bmatrix} = \begin{bmatrix}
3 \\
-4
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/hsc32rz5?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik P(3, 4) setelah direfleksikan ke sumbu X menjadi P'(3, -4).

### Contoh 2:

Jika kita memiliki titik Q(-2, 5), maka refleksi Q ke sumbu X adalah:

$$
Q' = A \cdot Q = \begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix} \cdot \begin{bmatrix}
-2 \\
5
\end{bmatrix} = \begin{bmatrix}
-2 \\
-5
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/muftjp5z?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik Q(-2, 5) setelah direfleksikan ke sumbu X menjadi Q'(-2, -5).

---

## Refleksi ke Sumbu Y

Refleksi ke sumbu Y memetakan setiap titik (x, y) ke (-x, y). Matriks yang merepresentasikan refleksi ini adalah:

$$
A = \begin{bmatrix}
-1 & 0 \\
0 & 1
\end{bmatrix}
$$

### Contoh 1:

Jika kita memiliki titik P(3, 4), maka refleksi P ke sumbu Y adalah:

$$
P' = A \cdot P = \begin{bmatrix}
-1 & 0 \\
0 & 1
\end{bmatrix} \cdot \begin{bmatrix}
3 \\
4
\end{bmatrix} = \begin{bmatrix}
-3 \\
4
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/hsc32rz5?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik P(3, 4) setelah direfleksikan ke sumbu Y menjadi P'(-3, 4).

### Contoh 2:

Jika kita memiliki titik Q(-1, 2), maka refleksi Q ke sumbu Y adalah:

$$
Q' = A \cdot Q = \begin{bmatrix}
-1 & 0 \\
0 & 1
\end{bmatrix} \cdot \begin{bmatrix}
-1 \\
2
\end{bmatrix} = \begin{bmatrix}
1 \\
2
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/njghhmk5?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik Q(-1, 2) setelah direfleksikan ke sumbu Y menjadi Q'(1, 2).

---

## Refleksi ke Sumbu X = Y

Refleksi ke sumbu X = Y memetakan setiap titik (x, y) ke (y, x). Matriks yang merepresentasikan refleksi ini adalah:

$$
A = \begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
$$

### Contoh 1:

Jika kita memiliki titik P(3, 4), maka refleksi P ke sumbu X = Y adalah:

$$
P' = A \cdot P = \begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix} \cdot \begin{bmatrix}
3 \\
4
\end{bmatrix} = \begin{bmatrix}
4 \\
3
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/gcsnqvss?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik P(3, 4) setelah direfleksikan ke sumbu X = Y menjadi P'(4, 3).

### Contoh 2:

Jika kita memiliki titik Q(5, -2), maka refleksi Q ke sumbu X = Y adalah:

$$
Q' = A \cdot Q = \begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix} \cdot \begin{bmatrix}
5 \\
-2
\end{bmatrix} = \begin{bmatrix}
-2 \\
5
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/rv8xrwvp?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik Q(5, -2) setelah direfleksikan ke sumbu X = Y menjadi Q'(-2, 5).

---

## Refleksi ke Sumbu Y = -X

Refleksi ke sumbu Y = -X memetakan setiap titik (x, y) ke (-y, -x). Matriks yang merepresentasikan refleksi ini adalah:

$$
A = \begin{bmatrix}
0 & -1 \\
-1 & 0
\end{bmatrix}
$$

### Contoh 1:

Jika kita memiliki titik P(3, 4), maka refleksi P ke sumbu Y = -X adalah:

$$
P' = A \cdot P = \begin{bmatrix}
0 & -1 \\
-1 & 0
\end{bmatrix} \cdot \begin{bmatrix}
3 \\
4
\end{bmatrix} = \begin{bmatrix}
-4 \\
-3
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/duxfp6jg?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik P(3, 4) setelah direfleksikan ke sumbu Y = -X menjadi P'(-4, -3).

### Contoh 2:

Jika kita memiliki titik Q(-2, 5), maka refleksi Q ke sumbu Y = -X adalah:

$$
Q' = A \cdot Q = \begin{bmatrix}
0 & -1 \\
-1 & 0
\end{bmatrix} \cdot \begin{bmatrix}
-2 \\
5
\end{bmatrix} = \begin{bmatrix}
-5 \\
2
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/bkwps2tw?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik Q(-2, 5) setelah direfleksikan ke sumbu Y = -X menjadi Q'(-5, 2).

---

## Refleksi ke Titik Asal (0,0)

Refleksi ke titik asal (0,0) memetakan setiap titik (x, y) ke (-x, -y). Matriks yang merepresentasikan refleksi ini adalah:

$$
A = \begin{bmatrix}
-1 & 0 \\
0 & -1
\end{bmatrix}
$$

### Contoh 1:

Jika kita memiliki titik P(3, 4), maka refleksi P ke titik asal adalah:

$$
P' = A \cdot P = \begin{bmatrix}
-1 & 0 \\
0 & -1
\end{bmatrix} \cdot \begin{bmatrix}
3 \\
4
\end{bmatrix} = \begin{bmatrix}
-3 \\
-4
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/arpgjye8?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik P(3, 4) setelah direfleksikan ke titik asal (0,0) menjadi P'(-3, -4).

### Contoh 2:

Jika kita memiliki titik Q(-1, 2), maka refleksi Q ke titik asal adalah:

$$
Q' = A \cdot Q = \begin{bmatrix}
-1 & 0 \\
0 & -1
\end{bmatrix} \cdot \begin{bmatrix}
-1 \\
2
\end{bmatrix} = \begin{bmatrix}
1 \\
-2
\end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/s5mh4rry?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik Q(-1, 2) setelah direfleksikan ke titik asal (0,0) menjadi Q'(1, -2).

---

## Kesimpulan

Transformasi refleksi adalah alat yang kuat dalam  aljabar linier. Dengan memahami cara kerja refleksi terhadap berbagai sumbu dan titik, kita dapat lebih baik dalam menganalisis dan memvisualisasikan perubahan dalam ruang vektor.