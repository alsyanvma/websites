<template>
    <footer class="bg-dark text-white py-4">
      <div class="container">
        <div class="row">
          <!-- Alamat -->
          <div class="col-md-6 mb-3">
            <h5>Alamat</h5>
            <p>
              Jl Depok Kel. Sukamenak Kec. Purbaratubratu <br>
              Kota Tasikmalaya.<br>
              Kode Pos: 46196. 
            </p>
            <i class="bi bi-telephone"> +62265312059</i><br> 
            <i class="bi bi-envelope"> info@smkn4-tsm.sch.id</i>
          </div>
  
          <!-- Media Sosial -->
          <div class="col-md-6 mb-3 text-md-end">
            <h5>Ikuti Kami</h5>
            <div class="social-icons">
              <!-- Facebook -->
              <a href="https://www.facebook.com/4smkn" class="text-white me-3" target="_blank" title="Facebook">
                <i class="bi bi-facebook"></i>
              </a>
              <!-- Instagram -->
              <a href="https://www.instagram.com/smkn4tasikmalaya/" class="text-white me-3" target="_blank" title="Instagram">
                <i class="bi bi-instagram"></i>
              </a>
            </div>
          </div>
        </div>
        <hr class="bg-white" />
        <p class="text-center mb-0">&copy; 2024 MyWebsite. All rights reserved.</p>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: "Footer",
  };
  </script>
  
  <style scoped>
  footer a:hover {
    text-decoration: underline;
  }
  
  .social-icons i {
    font-size: 1.5rem;
  }
  </style>
  