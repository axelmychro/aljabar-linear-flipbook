---
class: bg-[#303446] text-[#c6d0f5]
transition: fade
---

Determinan adalah sebuah fungsi luar biasa yang dalam arti tertentu mengukur keterbalikan (inversibilitas) dari suatu matriks berukuran n×n. Kita kemudian menyajikan rumus langsung, yang mengarah langsung pada pernyataan tentang keunikan dan sifat multiplikatif yang mengejutkan. [Determinan ternyata merupakan sebuah homomorfisma grup dari GLn​(k) ke k∗.] Terakhir, dari sifat multiplikatif ini, seseorang dapat dengan mudah menyimpulkan bahwa suatu matriks persegi dapat dibalik (memiliki invers) jika dan hanya jika determinannya tidak nol.

<div class="flex w-full h-[40%] border-2 border-[#e78284] items-center justify-evenly text-4xl">
  <div>

$A = \begin{pmatrix} 3 & 5 \\ 2 & 4 \end{pmatrix}$

  </div>

  <div>

$B = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 1 & 4 \\ 5 & 6 & 0 \end{pmatrix}$

  </div>
</div>

Kita akan coba cari determinan dari matriks 2\*2 dan 3\*3 berikut.

<!--Valenza, Robert J. Linear Algebra: An Introduction to Abstract Mathematics. Undergraduate Texts in Mathematics. New York: Springer-Verlag, 1993.-->

---
class: bg-[#303446] text-[#c6d0f5] text-2xl
transition: fade
---

<div class="flex flex-wrap w-full h-[80%] border-2 border-[#e78284] items-center text-4xl pl-8">
  <div class="text-6xl">

$A = \begin{pmatrix} 3 & 5 \\ 2 & 4 \end{pmatrix}$
  </div>

  <div>
$$
\det(A) = (3 \times 4) - (5 \times 2) = 12 - 10 = 2
$$

  </div>
</div>

Dengan metode persilangan, kita bisa menemukan determinan matriks 2\*2

---
class: bg-[#303446] text-[#c6d0f5]
transition: fade
---

<div class="flex flex-col w-full h-[80%] border-2 border-[#e78284] items-center justify-evenly text-2xl">

  <div>

$B = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 1 & 4 \\ 5 & 6 & 0 \end{pmatrix}$

  </div>
  
  <div class="absolute opacity-50 top-12 left-5/9">

$_ = \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ 5 & 6 \end{pmatrix}$

  </div>
  
  <div class="min-w-0.5 bg-[#e78284] top-12 left-130 min-h-32 absolute -rotate-45 z-50" />
  <div class="min-w-0.5 bg-[#e78284] top-12 left-140 min-h-32 absolute -rotate-45 z-50" />
  <div class="min-w-0.5 bg-[#e78284] top-12 left-150 min-h-32 absolute -rotate-45 z-50" />
  
  <div class="min-w-0.5 bg-[#e78284] top-12 left-130 min-h-32 absolute rotate-45 z-50" />
  <div class="min-w-0.5 bg-[#e78284] top-12 left-140 min-h-32 absolute rotate-45 z-50" />
  <div class="min-w-0.5 bg-[#e78284] top-12 left-150 min-h-32 absolute rotate-45 z-50" />
  <div>
  
$$
\begin{aligned}
\det(B) &= (1 \cdot 1 \cdot 0) + (2 \cdot 4 \cdot 5) + (3 \cdot 0 \cdot 6) \\
        &- (5 \cdot 1 \cdot 3) - (6 \cdot 4 \cdot 1) - (0 \cdot 0 \cdot 2) \\
\det(B) &= (0 + 40 + 0) - (15 + 24 + 0) \\
\det(B) &= 40 - 39 = 1
\end{aligned}
$$

  </div>
</div>

Metode Sarrus adalah cara visual yang sangat membantu untuk menghitung determinan matriks 3\*3. Namun, metode ini hanya berlaku untuk matriks 3\*3 dan tidak bisa digunakan untuk ukuran yang lain.
