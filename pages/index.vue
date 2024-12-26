<template>
    <div class="container-fluid">
      <div class="row my-5">
        <div class="col-lg-8 col-md-10 col-sm-12">
          <div class="card bg-foto rounded-5">
            <div class="card-body"></div>
          </div>
        </div>
      </div>
  
      
      <div class="image-text-wrapper">
        <div class="image-box">
          <picture>
            <img 
              src="assets/img/bapak.png" 
              alt="logo SMKN 4" 
              class="img-fluid logo-image" 
              width="200" 
              height="200">
          </picture>
        </div>
  
        <div class="text-container">
          <h1>Sambutan Kepala Sekolah</h1>
          <h2>
            Assalamualaikum Warahmatullahi Wabarakatuh<br><br>
            Selamat datang di SMKN 4 Tasikmalaya. Segala puji dan syukur kita panjatkan kehadirat Allah SWT, semoga kita semua ada dalam lindungan-Nya. Dan atas perkenan-Nya pula kami dapat menghadirkan website SMK Negeri 4 Tasikmalaya ini. Kami berharap dengan adanya website di SMK Negeri 4 Tasikmalaya ini para pengunjung dapat mengenal lebih jauh tentang sekolah kami sehingga dapat mempererat tali silaturrahmi antara sekolah dengan masyarakat demi kemajuan kita bersama. Tiada gading yang tak retak, website kami ini masih dalam proses pengembangan, masih banyak kekurangan yang harus kami perbaiki. Kritik dan sarannya yang membangun sangat kami harapkan untuk pengembangan ke depan.<br><br>
            Akhirnya, saya mengucapkan terimakasih yang sebesar-besarnya kepada semua pihak yang tidak dapat disebutkan satu persatu atas segala bantuan dan fasilitas yang telah diberikan. Semoga semua yang kita lakukan bermanfaat bagi masyarakat.<br><br>
            Wassalamu'alaikum Warahmatullahi Wabarakatuh.
          </h2>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  * {
    padding: 0;
    margin: 0;
  }
  
  .card {
    height: 400px;
    box-shadow: none;
    width: 100vw;
    max-width: none;
  }
  
  .card.bg-foto {
    background-image: url('../assets/img/kita.png');
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
  }
  
  h1, h2 {
    margin: 20px;
    padding: 0;
  }
  
  h1 {
    font-size: 24px;
    text-align: left;
    margin-top: 10px;
  }
  
  h2 {
    font-size: 16px;
    text-align: left;
    margin-top: 10px;
  }
  
  .image-text-wrapper {
    display: flex;
    align-items: flex-start;
  }
  
  .image-box {
    display: inline-block;
    padding: 10px;
    border: 2px solid #ddd;
    border-radius: 210px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    background-color: #fff;
    margin-right: 20px;
  }
  
  .text-container {
    max-width: 600px;
  }
  </style>
  