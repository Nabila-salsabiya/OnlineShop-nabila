<script setup>
import ProductCard from '../components/ProductCard.vue'
const daftarProduk = [
 { id: 1, nama: 'Kaos Sekolah', harga: 75000, gambar:
'https://tse4.mm.bing.net/th/id/OIP.TJu7CjzwViv3FxsM5e1yXQHaGh?r=0&pid=Api&P=0&h=180' },
 { id: 2, nama: 'Topi Sekolah', harga: 35000, gambar:
 'https://tse4.mm.bing.net/th/id/OIP.WbEOjPqgAW4UvAIvjxDQYwHaHa?r=0&pid=Api&P=0&h=180' },
{ id:3, nama: 'tas sekolah', harga: 850000, gambar:
'https://tse4.mm.bing.net/th/id/OIP.PIbaBCm5lczz3BGXu5PZPgHaHa?r=0&pid=Api&P=0&h=180' },
]
</script>
<template>
 <main>
 <h1>Produk Kami</h1>
 <div class="grid">
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
<style scoped>
.grid {
 display: flex;
 gap: 16px;
 flex-wrap: wrap;
}
</style>