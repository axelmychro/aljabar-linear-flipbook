---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Nilai Eigen dan Vektor Eigen

Ketika sebuah matriks $A$ dikalikan dengan suatu vektor $\mathbf{x}$, matriks tersebut bertindak sebagai **Transformasi Linear** yang dapat memutar, menarik, atau menekan vektor tersebut.

<p class="text-[#8aadf4] font-bold text-lg mt-6">Definisi Inti:</p>
Vektor Eigen (x) adalah vektor khusus yang arahnya <b>tidak berubah</b> (atau hanya berbalik arah) setelah ditransformasi oleh matriks $A$. Matriks tersebut hanya mengubah panjang vektornya sebesar faktor skala yang disebut Nilai Eigen.

$$A\mathbf{x} = \lambda\mathbf{x}$$

* $\mathbf{x}$: Vektor Eigen (syarat: $\mathbf{x} \neq \mathbf{0}$)
* $\lambda$: Nilai Eigen (berupa konstanta skalar)

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

## Persamaan Karakteristik & Diagonalisasi

$$A\mathbf{x} = \lambda I\mathbf{x}$$
$$(\lambda I - A)\mathbf{x} = 0$$

Agar persamaan memiliki solusi tak nol untuk $\mathbf{x}$, matriks $(\lambda I - A)$ tidak boleh memiliki invers. Ini menghasilkan <span class="text-[#8aadf4] font-bold">Persamaan Karakteristik</span>:

<div class="bg-[#8aadf4] bg-opacity-10 border border-[#8aadf4] text-center text-sm my-2">

$$ \det(\lambda I - A) = 0 $$
</div>

### Diagonalisasi Matriks
Jika matriks $n \times n$ memiliki $n$ vektor eigen yang bebas linear, ia dapat didiagonalisasi menjadi $A = PDP^{-1}$, dimana:
* $D$ adalah matriks diagonal yang berisi Nilai Eigen.
* $P$ adalah matriks yang kolom-kolomnya adalah Vektor Eigen.

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

## Contoh Soal: Penentuan Nilai Eigen

$$A = \begin{pmatrix} 4 & 1 \\ 2 & 3 \end{pmatrix}$$

**1. Bentuk $(\lambda I - A)$**
$$
\lambda I - A = \lambda \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} - \begin{pmatrix} 4 & 1 \\ 2 & 3 \end{pmatrix} = \begin{pmatrix} \lambda-4 & -1 \\ -2 & \lambda-3 \end{pmatrix}
$$

**2. Hitung Determinan (Persamaan Karakteristik)**
$$
\det(\lambda I - A) = (\lambda-4)(\lambda-3) - (-1)(-2) = 0
$$
$$
(\lambda^2 - 7\lambda + 12) - 2 = 0
$$
$$
\lambda^2 - 7\lambda + 10 = 0
$$

**3. Faktorkan untuk Mendapatkan Nilai Eigen**

$(\lambda - 5)(\lambda - 2) = 0$

<p class="absolute bottom-8 right-8 max-w-96">
Maka, Nilai Eigen-nya adalah 5 dan 2.
</p>