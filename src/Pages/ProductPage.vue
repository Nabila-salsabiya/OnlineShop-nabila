```vue
<script setup>
import ProductCard from '../components/ProductCard.vue'

const daftarProduk = [
  {
    id: 1,
    nama: 'Lipstik Diorr',
    harga: 750000,
    gambar:
      'https://i.pinimg.com/1200x/9f/a6/65/9fa6656e53402d7af42a96bd43bff541.jpg'
  },
  {
    id: 2,
    nama: 'Blush Diorrr',
    harga: 350000,
    gambar:
      'https://i.pinimg.com/736x/c1/48/39/c148393080af81ca87a83d14fc387666.jpg'
  },
  {
    id: 3,
    nama: 'Parfum Diorr',
    harga: 8500000,
    gambar:
      'https://i.pinimg.com/736x/07/71/ed/0771edee4246abc5f034c3be2e739e74.jpg'
  },
  {
    id: 4,
    nama: 'Set Make Up Diorr',
    harga: 10000000,
    gambar:
      'https://i.pinimg.com/736x/51/9e/7d/519e7df49d1200d19f0e45e175afda4c.jpg'
  }
]
</script>

<template>
  <main class="min-h-screen bg-gray-50 px-6 py-12">

    <!-- Judul -->
    <div class="text-center mb-10">
      <h1
        class="text-4xl md:text-5xl font-bold text-pink-600 mb-3"
      >
        Produk Kami
      </h1>

      <p class="text-gray-600 text-lg">
        Temukan produk pilihan terbaik untuk kebutuhanmu
      </p>
    </div>

    <!-- Daftar Produk -->
    <div
      class="max-w-7xl mx-auto
             grid grid-cols-1 sm:grid-cols-2
             lg:grid-cols-3 xl:grid-cols-4
             gap-6"
    >
      <ProductCard
        v-for="produk in daftarProduk"
        :key="produk.id"
        :nama="produk.nama"
        :harga="produk.harga"
        :gambar="produk.gambar"
      />
    </div>

  </main>
</template>
```
