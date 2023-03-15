<template>
  <div>
    <div class="row info mb-3">
      <h5 class="judul " style="display: flex;">
        <div class="brand-box"></div><span class="tulisann"> Layanan Akademik</span>
      </h5>
      <div class="col-md-4">
        <div class="justify-content-center py-auto">
          <div class="list-group teks">
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi1' }" @click="viu = 'opsi1'"
              aria-current="true">
              <i class="fa-regular fa-square-check"></i> Registrasi KRS
            </a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi2' }" @click="viu = 'opsi2'"><i
                class="fa-regular fa-square-check"></i>
              Ujian (UTS & UAS)</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi3' }" @click="viu = 'opsi3'"><i
                class="fa-regular fa-square-check"></i>
              Surat Keterangan Aktif</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi4' }" @click="viu = 'opsi4'"><i
                class="fa-regular fa-square-check"></i>
              Layanan Perkuliahan</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi5' }" @click="viu = 'opsi5'"><i
                class="fa-regular fa-square-check"></i>
              Ijazah & Transkip Nilai</a>
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi1" v-if="viu === 'opsi1'">
        <div class="card ">
          <div class="card-header k ">
            Registrasi KRS
          </div>
          <img class="foto card-img-top align-self-center" src="../assets/registrasi-krs.png" alt="">
          <div class="card-body l">
            Merupakan registrasi mahasiswa pada setiap semester awal perkuliahan
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi2" v-if="viu === 'opsi2'">
        <div class="card ">
          <div class="card-header k">
            Ujian (UTS & UAS)
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/akademik/uts-uas.png" alt="">
          <div class="card-body l">
            Layanan pengumuman jadwal kegiatan ujian akademik yang bertujuan untuk melakukan pengukuran dan penilaian
            kompetensi peserta didik, sebagai dasar kegiatan evaluasi pembelajaran perkuliahan.
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi3" v-if="viu === 'opsi3'">
        <div class="card ">
          <div class="card-header k">
            Surat Keterangan Aktif
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/akademik/surat-keterangan-aktif.png" alt="">
          <div class="card-body l">
            Layanan panduan pengajuan surat yang menjelaskan bahwa mahasiswa sebagaimana termaktub pada surat tersebut
            berstatus aktif mengikuti perkuliahan di semester tertentu.
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi4" v-if="viu === 'opsi4'">
        <div class="card ">
          <div class="card-header k">
            Layanan Perkuliahan
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/akademik/layanan-perkuliahan.png" alt="">
          <div class="card-body l">
            Layanan panduan mengenai proses pelayanan perkuliahan yang ada di IT Telkom Surabaya. </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi5" v-if="viu === 'opsi5'">
        <div class="card ">
          <div class="card-header k">
            Ijazah dan Transkrip Nilai
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/akademik/ijazah.png" alt="">
          <div class="card-body l">
            Layanan mengenai proses penerbitan transkrip dan ijazah kepada calon lulusan dan pihak terkait sehingga proses
            penerbitan transkrip dapat terkendali.
          </div>
        </div>
      </div>
    </div>

    <div class="row info mb-3">
      <h5 class="judul" style="display: flex;">
        <div class="brand-box"></div><span class="tulisann"> Informasi Akademik</span>
      </h5>
      <div class="col-md-6">
        <p class="desk">Merupakan unit yang bertugas mengelola administrasi akademik yang mencakup kegiatan layanan
          administrasi
          akademik, pusat bahasa, dan perpustakaan. Informasi lengkap mengenai Unit Akademik, silakan kunjungi:</p>
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
            <a class="links" href="https://akademik.ittelkom-sby.ac.id/">https://akademik.ittelkom-sby.ac.id/</a>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <img class="gambar" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/banner/device-academic.png" alt=""
          width="650px">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AkademikView',
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