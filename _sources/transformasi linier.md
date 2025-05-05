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

### Contoh:

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

<iframe src="https://www.geogebra.org/classic/hsc32rz5?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Jadi, titik P(3, 4) setelah direfleksikan ke sumbu X menjadi P'(3, -4).


<iframe src="https://www.geogebra.org/calculator/dat2aayf?embed" width="800" height="600" allowfullscreen style="border: 1px solidrgb(3, 3, 3);border-radius: 4px;" frameborder="0"></iframe>

## Refleksi ke Sumbu Y

<iframe src="https://www.geogebra.org/calculator/dat2aayf?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Refleksi ke Sumbu X = Y

<iframe src="https://www.geogebra.org/calculator/dat2aayf?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Refleksi ke Sumbu Y = -X

<iframe src="https://www.geogebra.org/calculator/dat2aayf?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Refleksi ke Titik Asal (0,0)

<iframe src="https://www.geogebra.org/calculator/dat2aayf?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>