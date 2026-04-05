---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

# Ruang Vektor

<p class="text-[#91d7e3] text-xl font-bold">Definisi Ruang Vektor</p>
Ruang vektor adalah himpunan objek (vektor) yang padanya didefinisikan dua operasi: <b>penjumlahan</b> dan <b>perkalian dengan skalar</b>. Operasi-operasi ini harus memenuhi 10 aksioma ruang vektor (seperti komutatif, asosiatif, keberadaan vektor nol, dll).

<div class="grid grid-cols-2 gap-4 mt-8">
<div class="border border-[#91d7e3] p-4 rounded-lg">
<h3 class="text-[#91d7e3] mb-2 font-bold">Basis</h3>
Himpunan vektor yang **merentang (span)** seluruh ruang vektor dan saling **bebas linear**. Ibarat "fondasi" minimal untuk membangun sebuah ruang.
</div>

<div class="border border-[#91d7e3] p-4 rounded-lg">
<h3 class="text-[#91d7e3] mb-2 font-bold">Dimensi</h3>
Jumlah vektor yang ada di dalam suatu Basis. Contoh: Ruang $R^3$ (3D) memiliki dimensi 3.
</div>
</div>

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

## Bebas Linear vs Bergantung Linear

Kumpulan vektor $v_1, v_2, \dots, v_n$ dikatakan <span class="text-[#91d7e3] font-bold">Bebas Linear</span> jika persamaan kombinasi linear:
$$c_1v_1 + c_2v_2 + \dots + c_nv_n = 0$$
**Hanya** memiliki solusi trivial, yaitu $c_1 = c_2 = \dots = c_n = 0$. 

Jika ada solusi lain selain nol, maka himpunan vektor tersebut disebut **Bergantung Linear** (salah satu vektor bisa dibentuk dari kombinasi vektor lainnya).

### Cara Praktis Cek Bebas Linear
Bentuk matriks dengan vektor-vektor tersebut sebagai kolom atau baris:
1. **Metode Determinan (Untuk matriks persegi):** Jika $\det(A) \neq 0$, maka bebas linear.
2. **Metode Reduksi Baris:** Jika setelah OBE tidak ada baris yang menjadi nol semua, maka bebas linear.

---
layout: default
class: bg-[#24273a] text-[#cad3f5]
---

## Contoh Soal: Analisis Bebas Linear

<p class="text-[#91d7e3] font-bold">Kasus:</p>
Apakah vektor-vektor berikut saling bebas linear?

$v_1 = (1, 2, 3)$, $v_2 = (0, 1, 2)$, dan $v_3 = (0, 0, 1)$ di $R^3$

**Penyelesaian (Metode Determinan):**
Susun vektor menjadi kolom matriks $A$:
$$
A = \begin{pmatrix}
1 & 0 & 0 \\
2 & 1 & 0 \\
3 & 2 & 1
\end{pmatrix}
$$

Karena matriks $A$ adalah matriks segitiga bawah, determinannya adalah hasil kali elemen diagonal utamanya:
$$ \det(A) = 1 \times 1 \times 1 = 1 $$

Karena $\det(A) \neq 0$, terbukti bahwa $v_1, v_2, v_3$ adalah himpunan vektor yang <span class="text-[#91d7e3] font-bold">Bebas Linear</span> dan dapat membentuk basis di $R^3$.