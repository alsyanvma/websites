<template>
    <div class="fasilitas">
      <h1>Fasilitas SMKN 4 Tasikmalaya</h1>
      <div class="video-container">
        <!-- Embed YouTube video -->
        <iframe 
          width="560" 
          height="315" 
          src="https://www.youtube.com/embed/5l2u9rHS36k" 
          frameborder="0" 
          allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
          allowfullscreen>
        </iframe>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Fasilitas"
  };
  </script>
  
  <style scoped>
  .fasilitas {
    text-align: center;
    margin-top: 20px;
  }
  
  .video-container {
    margin-top: 20px;
    max-width: 80%;
    margin-left: auto;
    margin-right: auto;
  }
  
  iframe {
    width: 100%;
    max-width: 800px;
    height: 450px;
  }
  </style>
  