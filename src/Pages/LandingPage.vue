<script setup lang="ts">
import router from '@/router';

</script>

<template>
    <main>
    <h1>Selamat datang di OnlineShop</h1>
    <p>Belanja gampang, mudah, dan lempang.</p>
    <video controls width="480" loop>
        <source src="https://www.w3schools.com/html/mov_bbb.mp4"/>
    </video>
    <button class="btn-grad">
        <RouterLink to="/product">lanjut beli</RouterLink>
    </button>
     </main>
     <div class="iyaa">
<h3>😍😍</h3>
<p>set make up dior</p>
     </div>
     <div class="iyaa">
        <h3>😍😍</h3>
        <p>Disini ada mke up dior ori</p>
        </div>
    </template>
    <style scoped>
video {
    margin-top: 16px;
    border-radius: 10px;
    display:block;
}
</style>