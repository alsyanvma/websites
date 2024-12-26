<template>
  <div class="ekstrakurikuler">
    <h1>Ekstrakurikuler SMKN 4 Tasikmalaya</h1>
    <div class="ekstrakurikuler-container">
      <div
        class="ekstrakurikuler-card"
        v-for="(ekskul, index) in ekstrakurikulerList"
        :key="index"
        @click="toggleDetail(index)"
      >
        <img :src="ekskul.image" alt="image" class="ekstrakurikuler-image" />
        <div class="card-content">
          <h2>{{ ekskul.name }}</h2>
          <p class="description">{{ ekskul.shortDescription }}</p>
        </div>
      </div>
    </div>
    <div
      v-if="selectedEkstrakurikuler !== null"
      class="ekstrakurikuler-detail"
    >
      <button @click="closeDetail" class="close-button">X</button>
      <h2>{{ selectedEkstrakurikuler.name }}</h2>
      <div class="detail-content">
        <div class="detail-images">
          <img
            v-for="(image, index) in selectedEkstrakurikuler.images"
            :key="index"
            :src="image"
            alt="ekstrakurikuler image"
            class="detail-image"
          />
        </div>
        <p>{{ selectedEkstrakurikuler.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Ekstrakurikuler",
  data() {
    return {
      ekstrakurikulerList: [
        {
          name: "Paskibra",
          image: "/assets/img/p.jpg", 
          shortDescription: "Ekstrakurikuler yang mengajarkan kedisiplinan dan kepemimpinan.",
          description: "Paskibra adalah ekstrakurikuler yang mengajarkan kedisiplinan, kepemimpinan, dan kecintaan terhadap tanah air melalui kegiatan baris berbaris.",
          images: [
            "/assets/img/paskibra1.jpg", 
            "/assets/img/paskibra2.jpg",
            "/assets/img/paskibra3.jpg"
          ]
        },
        {
          name: "Volleyball",
          image: "/assets/img/volley.jpg", 
          shortDescription: "Ekstrakurikuler untuk mengembangkan keterampilan bola voli.",
          description: "Ekstrakurikuler Volleyball mengembangkan keterampilan olahraga bola voli, serta kerjasama tim yang solid.",
          images: [
            "/assets/img/volley1.jpg", 
            "/assets/img/volley2.jpg",
            "/assets/img/volley3.jpg"
          ]
        },
        {
          name: "Basket",
          image: "/assets/img/basket.jpg",
          shortDescription: "Meningkatkan kemampuan bermain basket dan kerjasama tim.",
          description: "Ekstrakurikuler Basket mengajarkan teknik bermain basket dan meningkatkan kemampuan fisik serta kerjasama tim.",
          images: [
            "/assets/img/basket1.jpg", 
            "/assets/img/basket2.jpg",
            "/assets/img/basket3.jpg"
          ]
        }
      ],
      selectedEkstrakurikuler: null, 
    };
  },
  methods: {
    toggleDetail(index) {
      this.selectedEkstrakurikuler = this.ekstrakurikulerList[index];
    },
    closeDetail() {
      this.selectedEkstrakurikuler = null;
    }
  }
};
</script>

<style scoped>
.ekstrakurikuler {
  text-align: center;
  padding: 20px;
}

.ekstrakurikuler h1 {
  font-size: 32px;
  font-weight: bold;
  margin-bottom: 30px;
}

.ekstrakurikuler-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
}

.ekstrakurikuler-card {
  background-color: #f7f7f7;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
  transition: transform 0.3s ease;
  cursor: pointer;
}

.ekstrakurikuler-card:hover {
  transform: scale(1.05);
}

.ekstrakurikuler-image {
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

.description {
  font-size: 14px;
  color: #555;
  margin-top: 10px;
  line-height: 1.5;
}

.ekstrakurikuler-detail {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
  color: white;
  padding: 20px;
  overflow-y: auto;
}

.detail-content {
  text-align: center;
}

.detail-images {
  display: flex;
  justify-content: center;
  gap: 10px;
  margin-bottom: 20px;
}

.detail-image {
  width: 100px;
  height: 100px;
  object-fit: cover;
}

.close-button {
  position: absolute;
  top: 10px;
  right: 10px;
  background-color: #ff5e5e;
  border: none;
  color: white;
  font-size: 18px;
  padding: 10px;
  cursor: pointer;
}

.close-button:hover {
  background-color: #ff3b3b;
}
</style>
