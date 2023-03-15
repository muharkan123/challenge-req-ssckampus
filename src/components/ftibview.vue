<template>
  <div>
    <div class="row info mb-3">
      <h5 class="judul " style="display: flex;">
        <div class="brand-box"></div><span class="tulisann"> Layanan FTIB</span>
      </h5>
      <div class="col-md-4">
        <div class="justify-content-center py-auto">
          <div class="list-group teks">
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi1' }" @click="viu = 'opsi1'"
              aria-current="true">
              <i class="fa-regular fa-square-check"></i> Surat Keterangan Aktif Mahasiswa di Fakultas
            </a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi2' }" @click="viu = 'opsi2'"><i
                class="fa-regular fa-square-check"></i>
              Surat Pengantar dari Kampus untuk Tugas MK dan TA </a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi3' }" @click="viu = 'opsi3'"><i
                class="fa-regular fa-square-check"></i>
              Surat Dispensasi</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi4' }" @click="viu = 'opsi4'"><i
                class="fa-regular fa-square-check"></i>
              Surat Rekomendasi</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi5' }" @click="viu = 'opsi5'"><i
                class="fa-regular fa-square-check"></i>
              Surat Peminjaman Lab dan Perlengkapannya</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi6' }" @click="viu = 'opsi6'"><i
                class="fa-regular fa-square-check"></i>
              Residensi TA ( Mengina di kampus )</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi7' }" @click="viu = 'opsi7'"><i
                class="fa-regular fa-square-check"></i>
              Proposal Dana Kegiatan</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi8' }" @click="viu = 'opsi8'"><i
                class="fa-regular fa-square-check"></i>
              Legalisir KHS & Transkrip</a>
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi1" v-if="viu === 'opsi1'">
        <div class="card ">
          <div class="card-header k ">
            Surat Keterangan Aktif Mahasiswa di Fakultas 
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Surat_Keterangan_Aktif.png" alt="">
          <div class="card-body l">
            Layanan panduan pengajuan surat yang menjelaskan bahwa mahasiswa sebagaimana termaktub pada surat tersebut berstatus aktif mengikuti perkuliahan di semester tertentu 
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi2" v-if="viu === 'opsi2'">
        <div class="card ">
          <div class="card-header k">
            Surat Pengantar dari Kampus untuk Tugas MK dan TA 
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Surat_Keterangan_Aktif.png" alt="">
          <div class="card-body l">
            Surat pengantar yang dikeluarkan untuk Tugas Mata Kuliah dan Tugas Akhir untuk observasi ke suatu Instansi/perusahaan 
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi3" v-if="viu === 'opsi3'">
        <div class="card ">
          <div class="card-header k">
            Surat Dispensasi
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Surat_Keterangan_Aktif.png" alt="">
          <div class="card-body l">
            Surat resmi untuk keperluan meminta keringanan atau pemakluman dari suatu hal 
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi4" v-if="viu === 'opsi4'">
        <div class="card ">
          <div class="card-header k">
            Surat Rekomendasi
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Surat_Keterangan_Aktif.png" alt="">
          <div class="card-body l">
            Surat yang merekomendasikan mahasiswa atau disebut juga sebagai surat referensi yang membantu pihak ketiga mengetahui dan memahami lebih lanjut tentang mahasiswa tersebut  </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi5" v-if="viu === 'opsi5'">
        <div class="card ">
          <div class="card-header k">
            Surat Peminjaman Lab dan Perlengkapannya 
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Surat_Keterangan_Aktif.png" alt="">
          <div class="card-body l">
            Surat peminjaman ruangan atau inventaris laboratorium
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi6" v-if="viu === 'opsi6'">
        <div class="card ">
          <div class="card-header k">
            Residensi TA (menginap di kampus) 
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Surat_Keterangan_Aktif.png" alt="">
          <div class="card-body l">
            Surat keterangan dengan kepentingan menginap di kampus untuk keperluan Tugas Akhir 
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi7" v-if="viu === 'opsi7'">
        <div class="card ">
          <div class="card-header k">
            Proposal Dana Kegiatan
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Proposal_Dana_Kegiatan.png" alt="">
          <div class="card-body l">
            Sebuah dokumen rencana acara yang ditulis dengan tujuan permohonan izin dan dukungan berupa dana atau sponsor 
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi8" v-if="viu === 'opsi8'">
        <div class="card ">
          <div class="card-header k">
            Legalisir KHS & Transkrip 
          </div>
          <img class="foto card-img-top align-self-center"
            src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/fakultas/Legalisir_KHS.png" alt="">
          <div class="card-body l">
            Pembubuhan cap stempel dan tanda tangan asli oleh pihak yang berwenang pada lembar fotokopi Kartu Hasil Studi & Transkrip 
          </div>
        </div>
      </div>
    </div>

    <div class="row info mb-3">
      <h5 class="judul" style="display: flex;">
        <div class="brand-box"></div><span class="tulisann"> Informasi FTIB</span>
      </h5>
      <div class="col-md-6">
        <p class="desk">Merupakan unit yang bertugas mengelola administrasi ftib yang mencakup kegiatan layanan administrasi ftib, pusat bahasa, dan perpustakaan. Informasi lengkap mengenai Unit FTIB, silakan kunjungi:</p>
        <div class="row mb-3">
          <div class="col-md-1">
            <i class="fa-brands fa-instagram lgo"></i>
          </div>
          <div class="col-md-11">
            <a class="links" href="https://www.instagram.com/ftib.ittelkomsby/">ftib.ittelkomsby</a>
          </div>
        </div>
        <div class="row mt-3">
          <div class="col-md-1">
            <i class="fa-solid fa-globe lgo"></i>
          </div>
          <div class="col-md-11">
            <a class="links" href="https://ftib.ittelkom-sby.ac.id/">https://ftib.ittelkom-sby.ac.id/</a>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <img class="gambar" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/banner/device-ftib.png" alt=""
          width="650px">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FtibView',
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