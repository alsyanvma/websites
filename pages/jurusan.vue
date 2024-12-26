<template>
    <div class="jurusan">
      <h1>Jurusan SMKN 4 Tasikmalaya</h1>
      <div class="jurusan-container">
        <!-- Card untuk masing-masing jurusan -->
        <div class="jurusan-card" v-for="(jurusan, index) in jurusanList" :key="index">
          <img :src="jurusan.image" alt="image" class="jurusan-image" />
          <div class="card-content">
            <h2>{{ jurusan.name }}</h2>
            <p>{{ jurusan.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Jurusan",
    data() {
      return {
        // Data jurusan yang akan ditampilkan
        jurusanList: [
          {
            name: "PPLG (Pembangunan Perangkat Lunak dan Gim)",
            description: "Jurusan ini mempelajari tentang pengembangan perangkat lunak, aplikasi, dan permainan.",
            image: "/assets/img/pplg.jpg", // Ganti dengan path gambar yang sesuai
          },
          {
            name: "TKJ (Teknik Komputer dan Jaringan)",
            description: "Jurusan ini fokus pada pengelolaan jaringan komputer, instalasi, dan pemeliharaan perangkat keras.",
            image: "/assets/img/tkj.jpg", // Ganti dengan path gambar yang sesuai
          },
          {
            name: "TBSM (Teknik Bisnis Sepeda Motor)",
            description: "Jurusan yang mempelajari tentang perawatan dan perbaikan sepeda motor.",
            image: "/assets/img/tbsm.jpg", // Ganti dengan path gambar yang sesuai
          },
          {
            name: "TOI (Teknik Otomasi Industri)",
            description: "Jurusan yang mempelajari sistem otomasi dalam industri, termasuk robotik dan pengendalian mesin.",
            image: "/assets/img/toi.jpg", // Ganti dengan path gambar yang sesuai
          },
          {
            name: "DKV (Desain Komunikasi Visual)",
            description: "Jurusan yang fokus pada desain grafis, multimedia, dan komunikasi visual.",
            image: "/assets/img/dkv.jpg", // Ganti dengan path gambar yang sesuai
          }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .jurusan {
    text-align: center;
    padding: 20px;
  }
  
  .jurusan h1 {
    font-size: 32px;
    font-weight: bold;
    margin-bottom: 30px;
  }
  
  .jurusan-container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 20px;
  }
  
  .jurusan-card {
    background-color: #f7f7f7;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    transition: transform 0.3s ease;
  }
  
  .jurusan-card:hover {
    transform: scale(1.05);
  }
  
  .jurusan-image {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }
  
  .card-content {
    padding: 20px;
  }
  
  .card-content h2 {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 15px;
  }
  
  .card-content p {
    font-size: 16px;
    color: #666;
    margin-bottom: 20px;
  }
  </style>
  