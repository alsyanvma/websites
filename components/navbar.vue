<template>
  <header class="header-container">
    <div class="logo-container text-center">
      <picture>
        <img 
          src="assets/img/logo.png" 
          alt="logo SMKN 4" 
          class="img-fluid logo-image" 
          width="80" 
          height="80">
      </picture>
      <div class="school-name">SMKN 4 <br>TASIKMALAYA</div>
    </div>
    <nav class="navbar navbar-expand-lg">
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mx-auto">
          <li class="nav-item">
            <nuxt-link class="nav-link" to="/">Beranda</nuxt-link>
          </li>
          <li class="nav-item dropdown">
            
            <span class="nav-link dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
              Profil Sekolah
            </span>
            <div class="dropdown-menu">
              <nuxt-link class="dropdown-item" to="/visi-misi">Visi dan Misi</nuxt-link>
              <nuxt-link class="dropdown-item" to="/sejarah">Sejarah</nuxt-link>
              <nuxt-link class="dropdown-item" to="/fasilitas">Fasilitas</nuxt-link>
              <nuxt-link class="dropdown-item" to="/jurusan">Jurusan</nuxt-link>
            </div>
          </li>
          <li class="nav-item">
            <nuxt-link class="nav-link" to="/ekstrakurikuler">Ekstrakurikuler</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link class="nav-link" to="/galeri">Galeri</nuxt-link>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<style scoped>
/* Pusatkan keseluruhan tampilan halaman */
.header-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #f7f7f7;
  padding: 10px 10px;
}

.logo-container {
  text-align: center;
  margin-bottom: 10px;
}

.logo-image {
  margin-bottom: 10px;
}

.school-name {
  font-size: 20px;
  font-weight: bold;
  color: #333;
}

.navbar {
  background-color: #7a98be;
  color: #ffffff;
  padding: 10px 0;
  width: 100%;
}

.navbar-toggler {
  border: none;
}

.navbar-nav {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
}

.nav-item {
  margin: 0 15px;
  position: relative;
}

.nav-link {
  color: #ffffff;
  text-decoration: none;
}

.nav-link:hover {
  color: #ccc;
}

/* Dropdown menu */
.nav-item:hover .dropdown-menu {
  display: block;
}

.dropdown-menu {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  background-color: #7a98be;
  padding: 10px;
  border-radius: 5px;
}

.dropdown-item {
  color: #ffffff;
  text-decoration: none;
  padding: 5px 10px;
}

.dropdown-item:hover {
  background-color: #5a7f9e;
}

/* Responsivitas untuk layar kecil */
@media (max-width: 768px) {
  .nav-item {
    margin: 0 10px;
  }

  .school-name {
    font-size: 18px;
  }
}
</style>
