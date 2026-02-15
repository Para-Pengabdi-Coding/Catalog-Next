<template>
  <div class="page-shell">
    <!-- Hero Section -->
    <section class="relative overflow-hidden py-16 lg:py-24">
      <div class="absolute inset-0">
        <div
          class="absolute inset-0 bg-[url(https://media.johnlewiscontent.com/i/johnlewis/Small-space-furniture-lead)] bg-cover bg-center"
        ></div>
        <div class="absolute inset-0 bg-gradient-to-b from-slate-950/40 via-slate-900/60 to-slate-950/80"></div>
      </div>
      <UContainer class="relative grid gap-10 lg:grid-cols-[1.1fr_0.9fr] items-center text-white">
        <div class="space-y-6">
          <div class="flex items-center gap-3">
            <img src="/images/logo/asj.png" alt="Abadi Suar Jaya" class="w-16 md:w-20" />
            <div class="text-sm uppercase tracking-[0.3em] text-white/70">Abadi Suar Jaya</div>
          </div>
          <h1 class="display-title">Furniture elegan yang menenangkan ruang, dibuat rapi dari material pilihan.</h1>
          <p class="text-base md:text-lg text-white/80 max-w-xl">
            Rancang ulang suasana rumah dan kantor Anda dengan produk kayu berkualitas, desain modern, dan layanan yang
            jelas dari awal pemesanan hingga pengiriman.
          </p>
          <div class="flex flex-wrap gap-3">
            <UButton size="lg" to="/catalog" variant="solid" class="brand-button">Lihat Katalog</UButton>
            <UButton size="lg" to="/order" variant="outline" class="brand-button-outline text-white border-white/40">
              <span class="text-white"> Cara Pemesanan </span>
            </UButton>
          </div>
          <div class="grid grid-cols-2 md:grid-cols-4 gap-4 text-sm text-white/80">
            <div class="rounded-lg border border-white/10 bg-white/5 px-3 py-3">Produksi rapi & teliti</div>
            <div class="rounded-lg border border-white/10 bg-white/5 px-3 py-3">Bisa custom ukuran</div>
            <div class="rounded-lg border border-white/10 bg-white/5 px-3 py-3">Konsultasi desain</div>
            <div class="rounded-lg border border-white/10 bg-white/5 px-3 py-3">Pengiriman terjadwal</div>
          </div>
        </div>
        <div class="glass-panel rounded-2xl p-6 md:p-8 space-y-6">
          <div>
            <div class="section-kicker">Info Cepat</div>
            <h2 class="section-title text-white">Hubungi tim kami untuk estimasi cepat.</h2>
          </div>
          <div class="space-y-4 text-white/80 text-sm">
            <div class="flex items-center justify-between">
              <span>Jam Operasional</span>
              <span class="font-semibold text-white">09.00 - 17.00</span>
            </div>
            <div class="flex items-center justify-between">
              <span>Respon WhatsApp</span>
              <span class="font-semibold text-white">&lt; 2 jam</span>
            </div>
          </div>
          <div class="rounded-xl border border-white/10 bg-white/5 p-4 text-sm">
            Sertakan ukuran ruangan, preferensi warna, dan kebutuhan fungsi agar kami dapat memberi rekomendasi yang
            tepat.
          </div>
        </div>
      </UContainer>
    </section>

    <!-- Highlight -->
    <section class="section-gap">
      <UContainer>
        <div class="text-center mb-10">
          <div class="section-kicker">Keunggulan</div>
          <h2 class="section-title">Fokus pada kenyamanan, estetika, dan ketahanan.</h2>
          <p class="text-gray-600 max-w-2xl mx-auto mt-3">
            Kami menata pengalaman belanja furnitur agar jelas, informatif, dan mudah dipahami di semua perangkat.
          </p>
        </div>
        <div class="grid gap-4 md:grid-cols-3">
          <div class="card-soft rounded-2xl p-6 space-y-3">
            <div class="text-3xl">🪵</div>
            <h3 class="font-semibold text-lg">Material pilihan</h3>
            <p class="text-sm text-gray-600">
              Mengutamakan kayu berkualitas dengan finishing halus agar tahan lama dan mudah dirawat.
            </p>
          </div>
          <div class="card-soft rounded-2xl p-6 space-y-3">
            <div class="text-3xl">🧵</div>
            <h3 class="font-semibold text-lg">Detail rapi</h3>
            <p class="text-sm text-gray-600">
              Proses produksi diawasi ketat agar presisi sambungan, warna, dan hasil akhir konsisten.
            </p>
          </div>
          <div class="card-soft rounded-2xl p-6 space-y-3">
            <div class="text-3xl">📦</div>
            <h3 class="font-semibold text-lg">Pengiriman terencana</h3>
            <p class="text-sm text-gray-600">
              Estimasi waktu dan biaya dikomunikasikan di awal supaya pemesanan terasa aman.
            </p>
          </div>
        </div>
      </UContainer>
    </section>

    <!-- Tentang Usaha -->
    <section id="tentang" class="section-gap">
      <UContainer>
        <div class="flex flex-col gap-8 lg:grid lg:grid-cols-[1.2fr_0.8fr]">
          <div class="space-y-4">
            <div class="section-kicker">Profil</div>
            <h2 v-if="indonesian" class="section-title">Tentang Kami</h2>
            <h2 v-else class="section-title">About Us</h2>
            <div v-if="indonesian" class="space-y-3 text-gray-700">
              <p class="font-semibold text-lg">Salah satu meubel furniture terbaik di Kabupaten Banyuwangi.</p>
              <p>
                Meubel Abadi Suar Jaya berdiri sejak tahun 2010 dan berkomitmen menyediakan produk furniture berkualitas
                dengan harga terjangkau. Kami melayani set meja makan, meja kantor, berbagai macam kursi, serta pesanan
                custom sesuai kebutuhan Anda.
              </p>
              <p>
                Tim produksi kami memastikan setiap detail dikerjakan dengan teliti. Kenyamanan dan kepuasan pelanggan
                selalu menjadi prioritas utama.
              </p>
            </div>
            <div v-else class="space-y-3 text-gray-700">
              <p class="font-semibold text-lg">One of the best furniture manufacturers in Banyuwangi Regency.</p>
              <p>
                Meubel Abadi Suar Jaya, established in 2010, provides high-quality furniture at affordable prices. We
                deliver dining sets, office desks, various chairs, and custom orders tailored to your needs.
              </p>
              <p>
                Our production team ensures every detail is crafted carefully. Your comfort and satisfaction remain our
                top priority.
              </p>
            </div>
          </div>
          <div class="card-soft rounded-2xl p-6 space-y-4">
            <div class="section-kicker">Bantuan Bahasa</div>
            <div class="text-gray-700 text-sm">Pilih bahasa agar informasi lebih mudah dipahami.</div>
            <div class="flex items-center justify-center gap-3 text-sm">
              <div class="w-20 text-end">English</div>
              <USwitch v-model="indonesian" />
              <div class="w-20 text-start">Indonesia</div>
            </div>
            <div class="rounded-xl border border-slate-200 bg-white/60 p-4 text-sm text-gray-700">
              Dapatkan rekomendasi produk dengan menyebutkan ukuran ruangan, gaya interior, dan anggaran.
            </div>
          </div>
        </div>
      </UContainer>
    </section>

    <!-- Proses Singkat -->
    <section class="section-gap">
      <UContainer>
        <div class="text-center mb-10">
          <div class="section-kicker">Alur Pemesanan</div>
          <h2 class="section-title">Jelas sejak awal, tanpa kebingungan.</h2>
        </div>
        <div class="grid gap-4 md:grid-cols-3">
          <div class="card-soft rounded-2xl p-6">
            <div class="text-2xl font-semibold mb-2">1. Konsultasi</div>
            <p class="text-sm text-gray-600">Diskusikan kebutuhan ruang, ukuran, warna, dan estimasi waktu.</p>
          </div>
          <div class="card-soft rounded-2xl p-6">
            <div class="text-2xl font-semibold mb-2">2. Produksi</div>
            <p class="text-sm text-gray-600">Pengerjaan dimulai setelah pembayaran DP dan detail disepakati.</p>
          </div>
          <div class="card-soft rounded-2xl p-6">
            <div class="text-2xl font-semibold mb-2">3. Pengiriman</div>
            <p class="text-sm text-gray-600">Jadwal pengiriman dikonfirmasi sebelum produk dikirim.</p>
          </div>
        </div>
        <div class="mt-8 text-center">
          <UButton size="lg" to="/order" variant="solid" class="brand-button">Lihat Detail Cara Pemesanan</UButton>
        </div>
      </UContainer>
    </section>

    <!-- Keunggulan Usaha -->
    <section class="section-gap">
      <UContainer>
        <h2 v-if="indonesian" class="section-title text-center mb-10">Kenapa Memilih Kami?</h2>
        <h2 v-else class="section-title text-center mb-10">Why Choose Us?</h2>
        <div
          v-for="item in indonesian ? kelebihan : advantages"
          :key="item.title"
          class="card-soft rounded-2xl p-6 text-center mb-4"
        >
          <div class="text-4xl mb-3">{{ item.icon }}</div>
          <h3 class="font-bold mb-2">{{ item.title }}</h3>
          <p class="text-gray-600">{{ item.description }}</p>
        </div>
      </UContainer>
    </section>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "home",
});

const indonesian = ref(false);

const kelebihan = ref([
  {
    icon: "🪵",
    title: "Bahan Berkualitas",
    description: "Menggunakan kayu pilihan dan material terbaik.",
  },
  {
    icon: "🎨",
    title: "Desain Modern",
    description: "Mengikuti tren terbaru untuk keindahan rumah Anda.",
  },
  {
    icon: "⚡",
    title: "Pengiriman Cepat",
    description: "Proses pengiriman aman dan tepat waktu.",
  },
]);
const advantages = ref([
  {
    icon: "🪵",
    title: "High Quality",
    description: "Crafted from selected wood and premium materials.",
  },
  {
    icon: "🎨",
    title: "Modern Design",
    description: "Always following the latest trends to beautify your home.",
  },
  {
    icon: "⚡",
    title: "Fast Delivery",
    description: "Safe, reliable, and on-time shipping process.",
  },
]);
</script>

<style scoped>
.bg-primary-500 {
  background-color: #1e88e5;
}
.text-primary-500 {
  color: #1e88e5;
}
</style>
