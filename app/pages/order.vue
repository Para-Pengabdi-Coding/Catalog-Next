<template>
  <div class="page-shell">
    <!-- Hero -->
    <section class="section-gap text-center">
      <UContainer>
        <div class="section-kicker">Panduan Pemesanan</div>
        <h1 class="section-title">Cara pemesanan yang jelas, cepat, dan aman.</h1>
        <p class="text-gray-600 max-w-2xl mx-auto mt-3">
          Kami merancang alur pemesanan agar pengunjung memahami proses, estimasi waktu, serta biaya sejak awal.
        </p>
      </UContainer>
    </section>

    <!-- Steps -->
    <section class="section-gap pt-0">
      <UContainer>
        <UGrid :columns="[1, 2, 3]" gap="6">
          <UCard v-for="(step, index) in steps" :key="index" class="card-soft text-center p-6">
            <div class="text-4xl font-bold text-primary mb-4">{{ index + 1 }}</div>
            <h3 class="font-semibold text-lg mb-2">{{ step.title }}</h3>
            <p class="text-gray-600">{{ step.description }}</p>
          </UCard>
        </UGrid>
      </UContainer>
    </section>

    <!-- Notes -->
    <section class="section-gap pt-0">
      <UContainer>
        <div class="grid gap-6 lg:grid-cols-[1.2fr_0.8fr]">
          <div class="card-soft rounded-2xl p-6">
            <h2 class="text-xl font-semibold mb-4">Informasi yang Dibutuhkan</h2>
            <ul class="list-disc list-inside text-gray-600 space-y-2">
              <li>Ukuran ruang atau area penempatan (panjang x lebar x tinggi).</li>
              <li>Gaya desain yang diinginkan (minimalis, klasik, industrial, dll).</li>
              <li>Budget dan target waktu pengiriman.</li>
              <li>Referensi foto atau warna jika ada.</li>
            </ul>
          </div>
          <div class="card-soft rounded-2xl p-6">
            <h2 class="text-xl font-semibold mb-4">Catatan Penting</h2>
            <ul class="list-disc list-inside text-gray-600 space-y-2">
              <li>Waktu produksi ± 7-14 hari kerja tergantung jenis pesanan.</li>
              <li>Ongkos kirim ditanggung pembeli, disesuaikan dengan lokasi.</li>
              <li>Pembayaran DP minimal 50% dari total harga.</li>
              <li>Konfirmasi jadwal pengiriman dilakukan sebelum produk dikirim.</li>
            </ul>
          </div>
        </div>
      </UContainer>
    </section>

    <section class="section-gap pt-0">
      <UContainer>
        <div class="card-soft rounded-2xl p-6 md:p-8">
          <div class="section-kicker">Pembayaran & Pengiriman</div>
          <h2 class="section-title">Transparan sejak awal</h2>
          <div class="grid gap-4 md:grid-cols-3 mt-6 text-sm text-gray-600">
            <div>
              <div class="font-semibold text-gray-800">Metode pembayaran</div>
              <p>Transfer bank (BCA) atau pembayaran bertahap sesuai kesepakatan.</p>
            </div>
            <div>
              <div class="font-semibold text-gray-800">Estimasi biaya</div>
              <p>Biaya material, produksi, dan pengiriman dijelaskan sebelum produksi.</p>
            </div>
            <div>
              <div class="font-semibold text-gray-800">Update pengerjaan</div>
              <p>Tim kami memberikan kabar progres pada setiap tahap penting.</p>
            </div>
          </div>
        </div>
      </UContainer>
    </section>

    <!-- CTA -->
    <section class="section-gap">
      <UContainer>
        <div class="rounded-3xl bg-gradient-to-r from-slate-900 to-slate-800 text-white p-8 md:p-12 text-center">
          <h2 class="text-2xl md:text-3xl font-bold mb-4">Siap Memesan?</h2>
          <p class="mb-6 text-white/80">Klik tombol di bawah untuk langsung terhubung dengan kami via WhatsApp.</p>
          <div class="flex flex-col sm:flex-row gap-3 w-full justify-center items-center">
            <UButton
              size="lg"
              icon="i-mdi-whatsapp"
              variant="solid"
              class="brand-button"
              to="https://wa.me/+6285294775689?text=Halo, saya ingin membeli produk dari Meubel Abadi Suar Jaya"
              target="_blank"
            >
              Admin 1
            </UButton>
            <UButton
              size="lg"
              icon="i-mdi-whatsapp"
              variant="solid"
              class="brand-button"
              to="https://wa.me/+6285129870863?text=Halo, saya ingin membeli produk dari Meubel Abadi Suar Jaya"
              target="_blank"
            >
              Admin 2
            </UButton>
          </div>
        </div>
      </UContainer>
    </section>
  </div>
</template>

<script setup>
const steps = [
  {
    title: "Pilih Produk",
    description: "Telusuri katalog dan tentukan produk yang ingin Anda beli.",
  },
  {
    title: "Hubungi Kami",
    description: "Kirim detail pesanan ke WhatsApp kami untuk konfirmasi stok dan harga.",
  },
  {
    title: "Lakukan Pembayaran",
    description: "Transfer DP atau pembayaran penuh, lalu pesanan akan segera diproses.",
  },
];
</script>

<style scoped>
.bg-primary-500 {
  background-color: #1e88e5;
}
.text-primary {
  color: #1e88e5;
}
</style>
