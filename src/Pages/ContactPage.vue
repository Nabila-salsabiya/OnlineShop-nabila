```vue
<template>
  <div class="contact-page min-h-screen bg-gray-50">

    <!-- ==================== BANNER ==================== -->
    <section
      class="bg-gradient-to-r from-pink-300 to-pink-500
             text-white text-center
             py-12 px-4 shadow-md"
    >
      <h1
        class="text-4xl md:text-5xl
               font-bold tracking-wide"
      >
        Hubungi Kami
      </h1>

      <p class="mt-3 text-lg opacity-90">
        Kami siap membantu dan mendengarkan pesan dari kamu
      </p>
    </section>


    <!-- ==================== KONTEN UTAMA ==================== -->
    <section
      class="max-w-6xl mx-auto
             px-6 py-16
             grid grid-cols-1
             md:grid-cols-2
             gap-10"
    >

      <!-- ==================== INFO KONTAK ==================== -->
      <div
        class="bg-white rounded-2xl
               p-8 shadow-lg
               h-fit"
      >

        <h2
          class="text-3xl font-bold
                 text-pink-600 mb-6"
        >
          Info Kontak
        </h2>

        <ul class="space-y-5">

          <li
            class="flex items-start gap-3
                   text-gray-700 text-lg"
          >
            <span class="text-2xl">📍</span>
            <span>
              Jl. Bandung kota No 62
            </span>
          </li>

          <li
            class="flex items-start gap-3
                   text-gray-700 text-lg"
          >
            <span class="text-2xl">📞</span>
            <span>
              (813) 892184428
            </span>
          </li>

          <li
            class="flex items-start gap-3
                   text-gray-700 text-lg
                   break-all"
          >
            <span class="text-2xl">✉️</span>
            <span>
              info@SalsabiyaDIOR.com
            </span>
          </li>

        </ul>

        <!-- Jam Operasional -->
        <div
          class="mt-8 p-4
                 bg-pink-50
                 rounded-xl
                 border-l-4 border-pink-500"
        >
          <p class="text-gray-700 font-medium">
            🕐 Senin – Jumat
          </p>

          <p class="text-gray-600 mt-1">
            08.00 – 17.00
          </p>
        </div>

      </div>


      <!-- ==================== FORMULIR ==================== -->
      <div
        class="bg-white
               rounded-2xl
               p-8
               shadow-lg"
      >

        <h2
          class="text-3xl font-bold
                 text-pink-600 mb-6"
        >
          Kirim Pesan
        </h2>

        <form
          @submit.prevent
          class="space-y-5"
        >

          <!-- Nama -->
          <div>
            <label
              for="nama"
              class="block mb-2
                     font-semibold
                     text-gray-700"
            >
              Nama
            </label>

            <input
              id="nama"
              type="text"
              placeholder="Masukkan nama kamu"
              class="w-full
                     px-4 py-3
                     rounded-lg
                     border border-gray-300
                     text-gray-700
                     placeholder-gray-400
                     outline-none
                     transition duration-300
                     focus:border-pink-500
                     focus:ring-2
                     focus:ring-pink-200"
            />
          </div>


          <!-- Email -->
          <div>
            <label
              for="email"
              class="block mb-2
                     font-semibold
                     text-gray-700"
            >
              Email
            </label>

            <input
              id="email"
              type="email"
              placeholder="salsabiya@email.com"
              class="w-full
                     px-4 py-3
                     rounded-lg
                     border border-gray-300
                     text-gray-700
                     placeholder-gray-400
                     outline-none
                     transition duration-300
                     focus:border-pink-500
                     focus:ring-2
                     focus:ring-pink-200"
            />
          </div>


          <!-- Pesan -->
          <div>
            <label
              for="pesan"
              class="block mb-2
                     font-semibold
                     text-gray-700"
            >
              Pesan
            </label>

            <textarea
              id="pesan"
              rows="5"
              placeholder="Tulis pesan kamu di sini..."
              class="w-full
                     px-4 py-3
                     rounded-lg
                     border border-gray-300
                     text-gray-700
                     placeholder-gray-400
                     outline-none
                     resize-none
                     transition duration-300
                     focus:border-pink-500
                     focus:ring-2
                     focus:ring-pink-200"
            ></textarea>
          </div>


          <!-- Tombol Kirim -->
          <button
            type="submit"
            class="w-full
                   bg-pink-500
                   hover:bg-pink-600
                   text-white
                   font-semibold
                   py-3 px-6
                   rounded-full
                   shadow-md
                   transition duration-300
                   hover:-translate-y-1
                   hover:shadow-lg
                   cursor-pointer"
          >
            Kirim 🚀
          </button>

        </form>

      </div>

    </section>

  </div>
</template>

<script setup>
</script>
```

