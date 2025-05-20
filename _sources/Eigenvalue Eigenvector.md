# Eigenvalue dan Eigenvector

Eigenvalue adalah skalar yang menunjukkan faktor pengali yang diterapkan pada eigenvector ketika suatu matriks transformasi diterapkan, sedangkan eigenvector adalah vektor yang tetap pada arah yang sama meskipun ukurannya berubah ketika matriks tersebut diterapkan.

## Eigenvalue (Nilai Eigen)
Eigenvalue dari sebuah matriks A adalah skalar 
$$ \lambda $$
ynag memenuhi persamaan
---
$$ Av = \lambda v $$
---
dimana **v** adalah eigenvector yang sesuai.

## Eigenvector
Eigenvektor adalah vektor non-nol yang hanya diubah oleh matriks dengan skala, yaitu, ketika matriks diterapkan padanya, hasilnya adalah eigenvektor yang sama dikalikan dengan eigenvalue:
$$ Av = \lambda v $$

# Cara Mencari Eigenvalue dan Eigenvector

Misalkan kita menggunakan matriks berikut:

$$
A = \begin{bmatrix} 2 & 1 \\ 1 & 2 \end{bmatrix}
$$

## Langkah 1: Menentukan Eigenvalue

Eigenvalue $\lambda$ diperoleh dari:

$$
\det(A - \lambda I) = 0
$$

Dengan $I$ adalah matriks identitas. Maka:

$$
A - \lambda I = \begin{bmatrix} 2-\lambda & 1 \\ 1 & 2-\lambda \end{bmatrix}
$$

Hitung determinan:

$$
\det(A - \lambda I) = (2 - \lambda)(2 - \lambda) - 1 \cdot 1 = (2 - \lambda)^2 - 1
$$

$$
= 4 - 4\lambda + \lambda^2 - 1 = \lambda^2 - 4\lambda + 3
$$

Maka kita punya persamaan karakteristik:

$$
\lambda^2 - 4\lambda + 3 = 0
$$

###  Menyelesaikan persamaan kuadrat:

$$
\lambda = \frac{4 \pm \sqrt{(-4)^2 - 4 \cdot 1 \cdot 3}}{2 \cdot 1}
= \frac{4 \pm \sqrt{16 - 12}}{2}
= \frac{4 \pm \sqrt{4}}{2}
= \frac{4 \pm 2}{2}
$$

$$
\Rightarrow \lambda_1 = 3, \quad \lambda_2 = 1
$$

---

## Langkah 2: Mencari Eigenvector

Untuk masing-masing $\lambda$, kita cari $v$ yang memenuhi:

$$
(A - \lambda I)v = 0
$$

---

### Untuk $\lambda_1 = 3$:

$$
A - 3I = \begin{bmatrix} 2 - 3 & 1 \\ 1 & 2 - 3 \end{bmatrix}
= \begin{bmatrix} -1 & 1 \\ 1 & -1 \end{bmatrix}
$$

$$
\begin{bmatrix} -1 & 1 \\ 1 & -1 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix}
= \begin{bmatrix} 0 \\ 0 \end{bmatrix}
$$

Sistem persamaan:

$$
-1x + 1y = 0 \Rightarrow y = x
$$

Jadi eigenvector untuk $\lambda = 3$ adalah:

$$
v_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
\quad \text{(atau kelipatan skalar dari ini)}
$$

---

### Untuk $\lambda_2 = 1$:

$$
A - 1I = \begin{bmatrix} 2 - 1 & 1 \\ 1 & 2 - 1 \end{bmatrix}
= \begin{bmatrix} 1 & 1 \\ 1 & 1 \end{bmatrix}
$$

$$
\begin{bmatrix} 1 & 1 \\ 1 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix}
= \begin{bmatrix} 0 \\ 0 \end{bmatrix}
$$

$$
x + y = 0 \Rightarrow y = -x
$$

Jadi eigenvector untuk $\lambda = 1$ adalah:

$$
v_2 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}
\quad \text{(atau kelipatan skalar dari ini)}
$$

---

## Hasil Akhir

* **Eigenvalue**: $\lambda_1 = 3$, $\lambda_2 = 1$
* **Eigenvector**:
  * Untuk $\lambda = 3$: $\begin{bmatrix} 1 \\ 1 \end{bmatrix}$
  * Untuk $\lambda = 1$: $\begin{bmatrix} 1 \\ -1 \end{bmatrix}$