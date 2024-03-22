---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
css: unocss
---

# Dropship System di OnlineShop

(nama perusahaan disamarkan)

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---

# Business Model

<div grid="~ cols-2 gap-4">
<div>

- **OnlineShop** : Nama Perusahaan
- **Enabler** : Merchant dapat menjual barang dagangannya menggunakan sistem Dropship di OnlineShop, contoh : https://www.vinomofo.com/
- **Aggregator** : Sistem Dropship mendapat barang dagangan menggunakan API dari pihak ketiga, contoh : https://luxury-distribution.com/
- **Customer** : Pembeli membeli melalui website OnlineShop

</div>
<div>

```mermaid {theme: 'neutral', scale: 0.8}
graph TD
A[Enabler] -->|use our system| B((Dropship System))
    C[Aggregator] -->|our system using 3rd party provider| B
    B --> D[OnlineShop]
    D --> E([Customer])
```

</div>
</div>

<br>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
