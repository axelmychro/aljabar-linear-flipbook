---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Definisi Sistem Persamaan Linear

Sistem Persamaan Linear (SPL) adalah kumpulan dari dua atau lebih persamaan linear yang melibatkan variabel-variabel yang sama.

* **Linear**: Setiap variabel berpangkat satu. Tidak ada perkalian antar variabel (seperti $xy$).
* **Solusi**: Nilai-nilai variabel yang memenuhi **seluruh** persamaan dalam sistem secara serentak.
* **Himpunan Penyelesaian**: Kumpulan semua solusi yang mungkin. SPL bisa memiliki satu solusi unik, tak hingga solusi, atau tidak memiliki solusi sama sekali.

<div class="grid grid-cols-2 gap-4 mt-8">
<div class="border border-[#f5a97f] p-4 rounded-lg">
<h3 class="text-[#f5a97f] mb-2 font-bold">Contoh 2 Variabel</h3>

$$
\begin{cases} 
2x + 3y = 8 \\
x - y = 1 
\end{cases}
$$
</div>

<div class="border border-[#f5a97f] p-4 rounded-lg">
<h3 class="text-[#f5a97f] mb-2 font-bold">Contoh 3 Variabel</h3>

$$
\begin{cases} 
x + y + z = 6 \\
2x - y + z = 3 \\
x + 2y - z = 2
\end{cases}
$$
</div>
</div>

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Bentuk Matriks SPL

Representasi SPL dalam bentuk matriks memudahkan perhitungan komputasi dan analisis teoritis.

### Persamaan Matriks: <span class="text-[#f5a97f]">$A\mathbf{x} = \mathbf{b}$</span>

$$
\underbrace{
\begin{pmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{pmatrix}
}_{\text{Matriks Koefisien (A)}}
\underbrace{
\begin{pmatrix}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{pmatrix}
}_{\text{Vektor Variabel (x)}}
=
\underbrace{
\begin{pmatrix}
b_1 \\
b_2 \\
\vdots \\
b_m
\end{pmatrix}
}_{\text{Vektor Konstanta (b)}}
$$

### Matriks Diperbesar (*Augmented Matrix*)
Menggabungkan matriks koefisien dan vektor konstanta:
$$ [A|b] = \left( \begin{array}{ccc|c} a_{11} & a_{12} & a_{13} & b_1 \\ a_{21} & a_{22} & a_{23} & b_2 \\ a_{31} & a_{32} & a_{33} & b_3 \end{array} \right) $$

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Contoh Soal: Pemodelan SPL

<div class="bg-[#f5a97f] bg-opacity-10 border-l-4 border-[#f5a97f] p-4 my-4">
<p class="font-bold text-[#f5a97f]">Kasus:</p>
Sebuah pabrik memproduksi dua jenis barang, A dan B. Barang A membutuhkan 2 jam mesin pemotong dan 1 jam mesin perakit. Barang B membutuhkan 3 jam mesin pemotong dan 2 jam mesin perakit. Total waktu yang tersedia: 14 jam mesin pemotong dan 8 jam mesin perakit.
</div>

**1. Tentukan Variabel**
Misalkan $x_1$ = jumlah barang A, dan $x_2$ = jumlah barang B.

**2. Susun Sistem Persamaan Linear**
* Persamaan Mesin Pemotong: $2x_1 + 3x_2 = 14$
* Persamaan Mesin Perakit: $1x_1 + 2x_2 = 8$

**3. Ubah ke Bentuk Matriks Diperbesar**
$$
\left( \begin{array}{cc|c} 
2 & 3 & 14 \\ 
1 & 2 & 8 
\end{array} \right)
$$
*(Penyelesaian dari matriks ini akan dibahas pada materi Eliminasi Gauss).*