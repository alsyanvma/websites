<template>
  <div class="container my-5">
    <h2 class="text-center">Galeri Sekolah</h2>
    <div class="row">
      <div class="col-md-4" v-for="(image, index) in images" :key="index">
        <div class="card mb-4">
          <img :src="image.src" :alt="image.alt" class="card-img-top" />
          <div class="card-body">
            <h5 class="card-title">{{ image.title }}</h5>
            <p class="card-text">{{ image.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        {
          src: '/images/b1.jpg',
          alt: 'Kegiatan 1',
          title: 'Kegiatan Siswa 1',
          description: 'Maulid Nabi.',
        },
        {
          src: '/images/ima2.jpg',
          alt: 'Kegiatan 2',
          title: 'Kegiatan Siswa 2',
          description: 'Maulid Nabi.',
        },
        {
          src: '/images/image3.jpg',
          alt: 'Kegiatan 3',
          title: 'Kegiatan Siswa 3',
          description: 'Maulid Nabi.',
        },
      ],
    };
  },
};
</script>

<style scoped>
.card-img-top {
  object-fit: cover;
  height: 200px;
}
</style>
