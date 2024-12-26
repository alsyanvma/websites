<template>
  <div class="container">
    <h1 class="text">Visi & Misi</h1>
    <div class="ini visi">
      <h2>Visi</h2>
      <p class="highlight">Terwujudnya lulusan yang cerdas, aktif, kompetitif, adaptif, dan produktif berlandaskan iman dan takwa.</p>
    </div>
    <div class="ini misi">
      <h2>Misi</h2>
      <ul>
        <li>Menyiapkan Sumber Daya Manusia yang cerdas dan kompeten baik hardskill maupun softskill.</li>
        <li>Meningkatkan dan mengembangkan aktifitas serta kreatifitas seluruh warga sekolah dalam berbagai kegiatan positif.</li>
        <li>Mewujudkan manajemen pengelolaan yang efektif, efesien, transparan, akuntabel dan layanan prima.</li>
        <li>Menumbuhkan dan mengembangkan potensi dan kemampuan Sumber Daya Manusia yang berdaya saing tinggi melalui berbagai kegiatan akademik maupun non akademik.</li>
        <li>Menyelenggarakan berbagai program kegiatan dalam upaya meningkatkan Sumber Daya Manusia yang mampu menyesuaikan dengan perkembangan.</li>
        <li>Mengembangkan sarana prasarana dan lingkungan sekolah yang menyenangkan sebagai wadah menumbuhkembangkan daya kreasi dan inovasi untuk menghasilkan produk teknologi tepat guna.</li>
        <li>Membangun jiwa wirausaha yang handal melalui pembelajaran Teaching Factory (TEFA) dan Kelas Industri.        </li>
        <li>Menjalin dan mengembangkan kemitraan dengan Industri dan Dunia Kerja (IDUKA) serta lembaga lainnya yang relevan</li>
        <li>Menanamkan dan membudayakan sikap dan perilaku yang baik pada aktivitas di sekolah maupun dalam kehidupan sehari-hari.         </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'VisiMisi',
};
</script>

<style scoped>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  font-family: 'Arial', sans-serif;
}


.text {
  font-size: 36px;
  color: #2c6b38;
  text-align: center;
  margin-bottom: 30px;
  text-transform: uppercase;
  font-weight: bold;
}


.ini {
  background-color: #f8f8f8;
  padding: 30px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  margin-bottom: 30px;
}

h2 {
  font-size: 26px;
  color: #2c6b38;
  margin-bottom: 15px;
}

.highlight {
  font-size: 20px;
  font-weight: bold;
  color: #ff7043;
  text-align: center;
  margin-top: 15px;
}

ul {
  list-style-type: none;
  font-size: 18px;
  color: #333;
  padding-left: 20px;
}

li {
  margin-bottom: 12px;
  position: relative;
}

li:before {
  content: "•";
  position: absolute;
  left: -20px;
  color: #2c6b38;
}

@media (max-width: 768px) {
  .heading {
    font-size: 28px;
  }

  .section {
    padding: 20px;
  }

  ul {
    font-size: 16px;
  }

  .highlight {
    font-size: 18px;
  }
}
</style>