---
theme: default
title: Aljabar Linear Flipbook
info: |
  ## Aljabar Linear Flipbook
class: text-center
drawings:
  persist: false
transition: slide-left
comark: true
---

# Aljabar Linear Flipbook

Presentation slides for developers

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Press Space for next page <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

---
src: ./pages/i-daftar-isi.md
---

---
src:
./pages/1-matriks-dan-determinan.md
---

---
src:
./pages/2-sistem-persamaan-linear.md
---

---
src:
./pages/3-eliminasi-gauss.md
---

---
src:
./pages/4-vektor.md
---

---
src:
./pages/5-transformasi-linear.md
---

---