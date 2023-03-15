<template>
  <div>
    <div class="row info mb-3">
      <h5 class="judul" style="display: flex;">
        <div class="brand-box"></div><span class="tulisann"> Informasi Pusat Bahasa & Perpustakaan</span>
      </h5>
      <div class="col-md-6">
        <p class="desk">Merupakan unit yang bertugas mengelola administrasi perpus yang mencakup kegiatan layanan administrasi perpus, pusat bahasa, dan perpustakaan. Informasi lengkap mengenai Unit Pusat Bahasa & Perpustakaan, silakan kunjungi:</p>
        <div class="row mb-3">
          <div class="col-md-1">
            <i class="fa-brands fa-instagram lgo"></i>
          </div>
          <div class="col-md-11">
            <a class="links" href="https://www.instagram.com/akademikitts/">akademikitts</a>
          </div>
        </div>
        <div class="row mt-3">
          <div class="col-md-1">
            <i class="fa-solid fa-globe lgo"></i>
          </div>
          <div class="col-md-11">
            <a class="links" href="https://perpus.ittelkom-sby.ac.id/">https://perpus.ittelkom-sby.ac.id/</a>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <img class="gambar" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/banner/device-perpus.png" alt=""
          width="650px">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PerpusView',
  data() {
    return {
      viu: 'opsi1'
    }
  }
}
</script>

<style scoped>
.info {
  margin-top: 80px;
}

.links {
  font-size: 16px;
}

.lgo {
  color: rgb(170, 0, 0);
}

.desk {
  font-size: 15px;
  line-height: 24px;
  margin-bottom: 25px;
  font-weight: 400;
  color: #465b52;
}

.foto {
  width: 270px;
}

.k {
  font-size: 16px;
  font-weight: 700;
}

.l {
  font-size: 16px;
}

.brand-box {
  height: 1.2rem;
  width: 60px;
  background-color: rgb(170, 0, 0);
  border-radius: 0.3rem;
  margin-right: 20px;
  align-self: center;
}

.actives {
  background-color: rgb(170, 1, 1);
  color: white;
}

.tulisann {
  color: rgb(170, 1, 1);
}

.judul {
  font-family: 'League Spartan', sans-serif;
  font-weight: 600;
  font-size: 26px;
}

a {
  text-decoration: none;
  color: rgb(48, 47, 47);

}

.teks {
  font-size: 14px;
}</style>