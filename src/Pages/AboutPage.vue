```vue
<template>
  <div class="min-h-screen bg-gray-50">

    <!-- ==================== BANNER ==================== -->
    <section
      class="bg-gradient-to-r from-pink-300 to-pink-500
             text-white text-center
             py-12 px-4 shadow-md"
    >
      <h1
        class="text-4xl md:text-5xl font-bold tracking-wide"
      >
        Tentang Kami
      </h1>

      <p class="mt-3 text-lg opacity-90">
        Kenali lebih dekat toko dan tim kami
      </p>
    </section>


    <!-- ==================== CERITA KAMI ==================== -->
    <section class="py-16 px-6">

      <div
        class="max-w-6xl mx-auto
               flex flex-col md:flex-row
               items-center gap-10"
      >

        <!-- Teks -->
        <div class="flex-1">

          <h2
            class="text-3xl md:text-4xl font-bold
                   text-pink-600 mb-5"
          >
            Cerita Kami
          </h2>

          <p
            class="text-gray-600 text-base md:text-lg
                   leading-relaxed"
          >
            Toko kami berdiri dari kecintaan kami terhadap
            produk Dior dan set make up yang sangat bagus.
            Produk kami membantu memberikan hasil make up
            yang flawless dan elegan.

            <br /><br />

            Kami percaya bahwa setiap orang berhak mendapatkan
            produk make up yang berkualitas. Oleh karena itu,
            kami berusaha menyediakan produk pilihan dengan
            kualitas terbaik dan bahan yang terpercaya.
          </p>

          <!-- Tombol tambahan -->
          <button
            class="mt-6 bg-pink-500 text-white
                   px-6 py-3 rounded-full
                   font-semibold
                   shadow-md
                   transition duration-300
                   hover:bg-pink-600
                   hover:-translate-y-1
                   hover:shadow-lg"
          >
            Selengkapnya
          </button>

        </div>


        <!-- Gambar -->
        <div
          class="flex-1 flex justify-center
                 w-full"
        >
          <img
            src="https://i.pinimg.com/736x/30/06/d9/3006d9e3e80756becfb8bc410210fbb0.jpg"
            alt="Cerita Kami"
            class="w-full max-w-md
                   h-[350px]
                   object-cover
                   rounded-2xl
                   shadow-xl
                   transition duration-300
                   hover:scale-105"
          />
        </div>

      </div>

    </section>


    <!-- ==================== TIM KAMI ==================== -->
    <section
      class="py-16 px-6
             bg-pink-50
             text-center"
    >

      <h2
        class="text-3xl md:text-4xl
               font-bold text-pink-600"
      >
        Tim Kami
      </h2>

      <p
        class="mt-3 text-gray-600
               max-w-2xl mx-auto"
      >
        Kenali orang-orang yang berada di balik toko kami.
      </p>


      <!-- Grid Tim -->
      <div
        class="max-w-6xl mx-auto mt-10
               grid grid-cols-1
               sm:grid-cols-2
               lg:grid-cols-4
               gap-6"
      >

        <TeamCard
          v-for="anggota in daftarTim"
          :key="anggota.nama"
          :nama="anggota.nama"
          :jabatan="anggota.jabatan"
        />

      </div>

    </section>

  </div>
</template>


<script setup>
import { ref } from 'vue'
import TeamCard from '../components/TeamCard.vue'

// Data anggota tim
const daftarTim = ref([
  {
    nama: 'Nabila',
    jabatan: 'Project Manager'
  },
  {
    nama: 'Cinta',
    jabatan: 'Frontend Developer'
  },
  {
    nama: 'Kayla',
    jabatan: 'UI/UX Designer'
  },
  {
    nama: 'Alya',
    jabatan: 'Manager 2'
  }
])
</script>
```

