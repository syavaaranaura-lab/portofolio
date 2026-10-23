<script setup lang="ts">
import { ref } from 'vue'

const menuOpen = ref(false)

const closeMenu = () => {
  menuOpen.value = false
}

useSeoMeta({
  title: 'Raka Aditya — Atlet Renang',
  description: 'Portofolio Raka Aditya, atlet renang yang percaya setiap kayuhan membawa kita lebih dekat pada tujuan.',
})
</script>

<template>
  <main>
    <header class="site-header">
      <a class="brand" href="#beranda" aria-label="Raka Aditya, beranda" @click="closeMenu">
        <span class="brand-mark">R</span>
        <span>RAKA ADITYA<span class="brand-subtitle">SWIM PORTFOLIO</span></span>
      </a>

      <button
        class="menu-toggle"
        type="button"
        :aria-expanded="menuOpen"
        aria-label="Buka navigasi"
        @click="menuOpen = !menuOpen"
      >
        <span></span>
        <span></span>
      </button>

      <nav class="main-nav" :class="{ 'is-open': menuOpen }" aria-label="Navigasi utama">
        <a href="#tentang" @click="closeMenu">Tentang</a>
        <a href="#pencapaian" @click="closeMenu">Pencapaian</a>
        <a href="#galeri" @click="closeMenu">Galeri</a>
        <a class="nav-contact" href="#kontak" @click="closeMenu">Hubungi saya <span>↗</span></a>
      </nav>
    </header>

    <section id="beranda" class="hero">
      <div class="hero-image" role="img" aria-label="Atlet berenang di kolam renang"></div>
      <div class="hero-content">
        <p class="eyebrow"><span class="live-dot"></span> ATLET RENANG · JAKARTA, INDONESIA</p>
        <h1>Hidup<br />di antara<br /><span>dua napas.</span></h1>
        <p class="hero-copy">
          Saya Raka — perenang, pemimpi, dan pengejar garis finis berikutnya.
          Setiap kayuhan punya cerita.
        </p>
        <a class="button button-light" href="#tentang">Kenali perjalanan saya <span>↓</span></a>
      </div>
      <div class="hero-note"><span>01 / 04</span><span>FREESTYLE · BUTTERFLY</span></div>
      <div class="hero-side-label">BUILT IN THE WATER</div>
    </section>

    <section id="tentang" class="intro section-wrap">
      <div class="section-index"><span>01</span> TENTANG SAYA</div>
      <div class="intro-main">
        <p class="intro-lead">
          Kolam adalah tempat saya belajar bahwa <span>konsistensi mengalahkan bakat</span>
          ketika bakat berhenti berlatih.
        </p>
        <div class="intro-bottom">
          <p>
            Saya mulai berenang sejak usia 8 tahun. Kini, lebih dari satu dekade di dalam air
            mengajarkan saya tentang disiplin, keberanian, dan menikmati proses — bukan hanya podium.
          </p>
          <div class="personal-data">
            <div><span>DOMISILI</span><strong>Jakarta, Indonesia</strong></div>
            <div><span>SPESIALISASI</span><strong>Gaya bebas & kupu-kupu</strong></div>
            <div><span>KLUB</span><strong>Jakarta Aquatic Club</strong></div>
          </div>
        </div>
      </div>
      <div class="intro-photo">
        <img
          src="https://images.unsplash.com/photo-1530549387789-4c1017266635?auto=format&fit=crop&w=1000&q=85"
          alt="Lintasan kolam renang berwarna biru"
          loading="lazy"
        />
        <span>RUTINITAS PAGI, 05:30</span>
      </div>
    </section>

    <section id="pencapaian" class="achievements">
      <div class="section-wrap">
        <div class="section-index section-index-light"><span>02</span> ANGKA & PENCAPAIAN</div>
        <div class="achievement-heading">
          <h2>Bukan cuma<br /><em>tentang medali.</em></h2>
          <p>Setiap angka menyimpan ribuan jam latihan, hari-hari sulit, dan orang-orang yang percaya.</p>
        </div>
        <div class="stats-grid">
          <article class="stat-card">
            <span class="stat-number">12<span>+</span></span>
            <span class="stat-label">TAHUN BERENANG</span>
            <p>Dari kelas pemula hingga kompetisi nasional.</p>
          </article>
          <article class="stat-card">
            <span class="stat-number">08</span>
            <span class="stat-label">MEDALI NASIONAL</span>
            <p>Hasil dari kerja keras bersama tim terbaik.</p>
          </article>
          <article class="stat-card">
            <span class="stat-number">52<span>s</span></span>
            <span class="stat-label">50M GAYA BEBAS</span>
            <p>Personal best — dan masih terus ditantang.</p>
          </article>
          <article class="stat-card">
            <span class="stat-number">06</span>
            <span class="stat-label">KOMPETISI INTERNASIONAL</span>
            <p>Belajar membawa Merah Putih lebih jauh.</p>
          </article>
        </div>
        <div class="record-row">
          <span>CATATAN TERBARU</span>
          <strong>Kejuaraan Renang Nasional 2024</strong>
          <span>EMAS · 100M GAYA BEBAS</span>
          <span>01:02.48</span>
        </div>
      </div>
    </section>

    <section class="journey section-wrap">
      <div class="section-index"><span>03</span> PERJALANAN</div>
      <div class="journey-content">
        <h2>Langkah kecil.<br /><span>Kayuhan besar.</span></h2>
        <div class="timeline">
          <article class="timeline-item">
            <span class="timeline-year">2012</span>
            <div><h3>Semua dimulai</h3><p>Pertama kali masuk klub renang. Air terasa dingin, tapi saya tahu ini tempat saya.</p></div>
            <span class="timeline-tag">JAKARTA</span>
          </article>
          <article class="timeline-item">
            <span class="timeline-year">2017</span>
            <div><h3>Podium pertama</h3><p>Medali perunggu di kejuaraan tingkat provinsi. Rasanya? Lebih baik dari yang dibayangkan.</p></div>
            <span class="timeline-tag">JUNIOR</span>
          </article>
          <article class="timeline-item">
            <span class="timeline-year">2021</span>
            <div><h3>Level berikutnya</h3><p>Bergabung dengan tim senior dan mulai berkompetisi di kejuaraan nasional.</p></div>
            <span class="timeline-tag">SENIOR</span>
          </article>
          <article class="timeline-item">
            <span class="timeline-year">2024</span>
            <div><h3>Rekor baru</h3><p>Emas nasional di nomor 100 meter gaya bebas. Ini baru permulaan.</p></div>
            <span class="timeline-tag">NASIONAL</span>
          </article>
        </div>
      </div>
    </section>

    <section id="galeri" class="gallery-section">
      <div class="section-wrap">
        <div class="section-index"><span>04</span> DI BALIK LINTASAN</div>
        <div class="gallery-heading">
          <h2>Lebih dari<br /><em>sekadar berenang.</em></h2>
          <p>Momen-momen kecil yang membuat semuanya berarti.</p>
        </div>
        <div class="gallery-grid">
          <figure class="gallery-large">
            <img
              src="https://images.unsplash.com/photo-1576013551627-0cc20b96c2a7?auto=format&fit=crop&w=1200&q=85"
              alt="Air kolam renang biru dilihat dari atas"
              loading="lazy"
            />
            <figcaption><span>01</span> THE DAILY GRIND</figcaption>
          </figure>
          <figure class="gallery-small">
            <img
              src="https://images.unsplash.com/photo-1560090995-01632a28895b?auto=format&fit=crop&w=900&q=85"
              alt="Kolam renang saat matahari terbit"
              loading="lazy"
            />
            <figcaption><span>02</span> BEFORE SUNRISE</figcaption>
          </figure>
          <div class="gallery-quote">
            <span>“</span>
            <p>Jangan hitung putaran. Buat setiap putaran berarti.</p>
            <small>CATATAN DARI PELATIH</small>
          </div>
        </div>
      </div>
    </section>

    <footer id="kontak" class="contact-section">
      <div class="section-wrap">
        <div class="section-index section-index-light"><span>05</span> KOLABORASI & KONTAK</div>
        <p class="contact-kicker">PUNYA CERITA DI AIR?</p>
        <h2>Mari bikin<br /><em>gelombang.</em></h2>
        <a class="contact-link" href="mailto:halo@rakaaditya.com">
          halo@rakaaditya.com <span>↗</span>
        </a>
        <div class="footer-bottom">
          <a class="brand footer-brand" href="#beranda">
            <span class="brand-mark">R</span>
            <span>RAKA ADITYA<span class="brand-subtitle">SWIM PORTFOLIO</span></span>
          </a>
          <span>© 2025 RAKA ADITYA · DIBUAT DENGAN DEDIKASI</span>
          <a class="back-top" href="#beranda">KEMBALI KE ATAS ↑</a>
        </div>
      </div>
    </footer>
  </main>
</template>
