<template>
  <div>
    <div class="row info mb-3">
      <h5 class="judul " style="display: flex;">
        <div class="brand-box"></div><span class="tulisann"> Layanan Keuangan</span>
      </h5>
      <div class="col-md-4">
        <div class="justify-content-center py-auto">
          <div class="list-group teks">
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi1' }" @click="viu = 'opsi1'"
              aria-current="true">
              <i class="fa-regular fa-square-check"></i> Pembayaran BPP Semester
            </a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi2' }" @click="viu = 'opsi2'"><i
                class="fa-regular fa-square-check"></i>
              Pengajuan Angsuran</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi3' }" @click="viu = 'opsi3'"><i
                class="fa-regular fa-square-check"></i>
              Permintaan Bukti Pembayaran/Kuitansi Pembayaran Biaya Pendidikan</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi4' }" @click="viu = 'opsi4'"><i
                class="fa-regular fa-square-check"></i>
              Permintaan Surat Tagihan/Invoice Biaya Pendidikan</a>
            <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi5' }" @click="viu = 'opsi5'"><i
                class="fa-regular fa-square-check"></i>
              Permintaan Surat Keterangan Bebas Administrasi Keuangan</a>
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi1" v-if="viu === 'opsi1'">
        <div class="card ">
          <div class="card-header k ">
            Pembayaran BPP Semester
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/keuangan/Pembayaran_BPP_Semester.png" alt="">
          <div class="card-body l">
            Panduan pembayaran Biaya Penyelenggaraan Pendidikan setiap semester.
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi2" v-if="viu === 'opsi2'">
        <div class="card ">
          <div class="card-header k">
            Pengajuan Angsuran
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/keuangan/Pengajuan_Angsuran.png" alt="">
          <div class="card-body l">
            Pengajuan keringanan bagi mahasiswa yang belum dapat melakukan pelunasan pembayaran BPP
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi3" v-if="viu === 'opsi3'">
        <div class="card ">
          <div class="card-header k">
            Permintaan Bukti Pembayaran/Kuitansi Pembayaran Biaya Pendidikan
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/keuangan/Permintaan_Bukti_Pembayaran.png" alt="">
          <div class="card-body l">
            Permintaan bukti pembayaran biaya pendidikan dari mahasiswa atau orang tua/wali mahasiswa
          </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi4" v-if="viu === 'opsi4'">
        <div class="card ">
          <div class="card-header k">
            Permintaan Surat Tagihan/ Invoice Biaya Pendidikan 
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/keuangan/Permintaan_Surat_Tagihan.png" alt="">
          <div class="card-body l">
            Permintaan surat tagihan atau invoice biaya pendidikan dari mahasiswa atau orang tua/wali mahasiswa  </div>
        </div>
      </div>
      <div class="col-md-8" id="opsi5" v-if="viu === 'opsi5'">
        <div class="card ">
          <div class="card-header k">
            Permintaan Surat Keterangan Bebas Administrasi Keuangan
          </div>
          <img class="foto card-img-top align-self-center" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/keuangan/Permintaan_Surat_Keterangan.png" alt="">
          <div class="card-body l">
            Permintaan surat keterangan yang menyatakan bahwa mahasiswa sudah tidak memiliki piutang biaya pendidikan. Surat tersebut digunakan untuk keperluan mengurus proses kelulusan dan proses undur diri 
          </div>
        </div>
      </div>
    </div>

    <div class="row info mb-3">
      <h5 class="judul" style="display: flex;">
        <div class="brand-box"></div><span class="tulisann"> Informasi Keuangan</span>
      </h5>
      <div class="col-md-6">
        <p class="desk">Merupakan unit yang bertugas mengelola administrasi keuangan yang mencakup kegiatan layanan administrasi keuangan, pusat bahasa, dan perpustakaan. Informasi lengkap mengenai Unit Keuangan, silakan kunjungi:</p>
        <div class="row mb-3">
          <div class="col-md-1">
            <i class="fa-brands fa-instagram lgo"></i>
          </div>
          <div class="col-md-11">
            <a class="links" href="https://www.instagram.com/keuangan.ittelkomsby/">keuangan.ittelkomsby</a>
          </div>
        </div>
        <div class="row mt-3">
          <div class="col-md-1">
            <i class="fa-solid fa-globe lgo"></i>
          </div>
          <div class="col-md-11">
            <a class="links" href="https://keuangan.ittelkom-sby.ac.id/">https://keuangan.ittelkom-sby.ac.id/</a>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <img class="gambar" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/banner/device-keuangan.png" alt=""
          width="650px">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'KeuanganView',
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