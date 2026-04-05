---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Metode Eliminasi Gauss & Gauss-Jordan

Tujuan utama metode ini adalah menyederhanakan *Augmented Matrix* menggunakan **Operasi Baris Elementer (OBE)** agar nilai variabel mudah ditemukan.

<div class="border border-[#a6da95] p-4 rounded-lg my-4">
<h3 class="text-[#a6da95] mb-2 font-bold">Tiga Aturan OBE:</h3>
<ol class="list-decimal pl-6">
  <li><b>Pertukaran</b>: Menukar posisi dua baris ($R_i \leftrightarrow R_j$).</li>
  <li><b>Perkalian</b>: Mengalikan baris dengan konstanta tak nol ($k \cdot R_i$).</li>
  <li><b>Penjumlahan</b>: Menambahkan kelipatan suatu baris ke baris lain ($R_i + kR_j \rightarrow R_i$).</li>
</ol>
</div>

* **Eliminasi Gauss**: Menghasilkan **Bentuk Eselon Baris** (Matriks Segitiga Atas). Membutuhkan *Substitusi Mundur* di akhir.
* **Eliminasi Gauss-Jordan**: Menghasilkan **Bentuk Eselon Baris Terreduksi** (Matriks Identitas). Solusi langsung terbaca tanpa substitusi.

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Contoh Penyelesaian: Eliminasi Gauss

<p class="text-[#a6da95] font-bold">Soal:</p> Selesaikan sistem persamaan berikut:
$x + y + z = 6$ <br>
$2x - y + 3z = 14$ <br>
$-x + 2y - z = -2$

**Langkah 1: Tulis Matriks Diperbesar**
$$
\left( \begin{array}{ccc|c} 
1 & 1 & 1 & 6 \\ 
2 & -1 & 3 & 14 \\ 
-1 & 2 & -1 & -2 
\end{array} \right)
$$

**Langkah 2: Operasi Baris Elementer (Membentuk Segitiga Atas)**
* $R_2 - 2R_1 \rightarrow R_2$ dan $R_3 + R_1 \rightarrow R_3$:
$$
\left( \begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & -3 & 1 & 2 \\ 0 & 3 & 0 & 4 \end{array} \right)
$$
* $R_3 + R_2 \rightarrow R_3$:
$$
\left( \begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & -3 & 1 & 2 \\ 0 & 0 & 1 & 6 \end{array} \right)
$$

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Lanjutan: Substitusi Mundur & Gauss-Jordan

<p class="text-[#a6da95] font-bold">Substitusi Mundur (Dari Eliminasi Gauss):</p>
Dari matriks terakhir, kita dapatkan:
1. $z = 6$
2. $-3y + z = 2 \Rightarrow -3y + 6 = 2 \Rightarrow -3y = -4 \Rightarrow y = 4/3$
3. $x + y + z = 6 \Rightarrow x + 4/3 + 6 = 6 \Rightarrow x = -4/3$

<hr class="border-[#a6da95] my-6 opacity-30">

<p class="text-[#a6da95] font-bold">Bagaimana jika dilanjutkan ke Gauss-Jordan?</p>
Target kita adalah mengubah matriks menjadi matriks identitas. Dari bentuk sebelumnya:
$$
\left( \begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & 1 & -1/3 & -2/3 \\ 0 & 0 & 1 & 6 \end{array} \right) \xrightarrow{\text{Hilangkan angka di atas diagonal}} \left( \begin{array}{ccc|c} 1 & 0 & 0 & -4/3 \\ 0 & 1 & 0 & 4/3 \\ 0 & 0 & 1 & 6 \end{array} \right)
$$

Hasilnya sama, namun Gauss-Jordan lebih panjang dalam matriks, sedangkan Gauss membutuhkan hitungan aljabar di luar matriks.