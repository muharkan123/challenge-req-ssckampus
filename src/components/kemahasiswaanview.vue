<template>
    <div>
        <div class="row info mb-3">
            <h5 class="judul " style="display: flex;">
                <div class="brand-box"></div><span class="tulisann"> Layanan Kemahasiswaan</span>
            </h5>
            <div class="col-md-4">
                <div class="justify-content-center py-auto">
                    <div class="list-group teks">
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi1' }" @click="viu = 'opsi1'"
                            aria-current="true">
                            <i class="fa-regular fa-square-check"></i> Transkrip aktivitas kemahasiswaan (TAK)
                        </a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi2' }" @click="viu = 'opsi2'"><i
                                class="fa-regular fa-square-check"></i>
                            Surat Tugas / Dispensasi</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi3' }" @click="viu = 'opsi3'"><i
                                class="fa-regular fa-square-check"></i>
                            Surat Rekomendasi / Delegasi Lomba</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi4' }" @click="viu = 'opsi4'"><i
                                class="fa-regular fa-square-check"></i>
                            Surat Keterangan Beasiswa</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi5' }" @click="viu = 'opsi5'"><i
                                class="fa-regular fa-square-check"></i>
                            KTM, Jas Almamater, dan Vest</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi6' }" @click="viu = 'opsi6'"><i
                                class="fa-regular fa-square-check"></i>
                            Proposal Pengajuan Dana dan LPJ Kegiatan Ormawa dan UKM</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi7' }" @click="viu = 'opsi7'"><i
                                class="fa-regular fa-square-check"></i>
                            Asuransi dan Layanan Kesehatan Telkomedika</a>
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi1" v-if="viu === 'opsi1'">
                <div class="card ">
                    <div class="card-header k ">
                        Transkrip aktivitas kemahasiswaan (TAK)
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/kemahasiswaan/tak.png" alt="">
                    <div class="card-body l">
                        Layanan approval sertifikat TAK sebagai syarat untuk mengikuti sidang tugas akhir/skripsi/proyek akhir, mendapatkan beasiswa, dan mengikuti seleksi mahasiswa berprestasi.
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi2" v-if="viu === 'opsi2'">
                <div class="card ">
                    <div class="card-header k">
                        Surat Tugas / Dispensasi
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/kemahasiswaan/surat-dispen.png" alt="">
                    <div class="card-body l">
                        Layanan pembuatan surat tugas atau dispensasi untuk kebutuhan presensi.
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi3" v-if="viu === 'opsi3'">
                <div class="card ">
                    <div class="card-header k">
                        Surat Rekomendasi / Delegasi Lomba
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/kemahasiswaan/surat-lomba.png" alt="">
                    <div class="card-body l">
                        Layanan pengajuan surat rekomendasi atau surat pengantar lomba. </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi4" v-if="viu === 'opsi4'">
                <div class="card ">
                    <div class="card-header k">
                        Surat Keterangan Tidak Menerima Beasiswa dari Kampus
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/kemahasiswaan/surat-beasiswa.png" alt="">
                    <div class="card-body l">
                        Layanan pembuatan surat keterangan tidak menerima beasiswa dari kampus untuk keperluan tertentu. 
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi5" v-if="viu === 'opsi5'">
                <div class="card ">
                    <div class="card-header k">
                        KTM, Jas Almamater dan Vest
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/kemahasiswaan/ktm.png" alt="">
                    <div class="card-body l">
                        Layanan pendataan, penerimaan jas almamater & vest serta KTM mahasiswa Institut Teknologi Telkom Surabaya. 
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi6" v-if="viu === 'opsi6'">
                <div class="card ">
                    <div class="card-header k">
                        Proposal Pengajuan Dana dan LPJ Kegiatan Ormawa dan UKM
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/kemahasiswaan/proposal-pengajuan.png" alt="">
                    <div class="card-body l">
                        Layanan terkait pelaksanaan pengusulan & pendanaan program kegiatan ormawa dan UKM. 
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi7" v-if="viu === 'opsi7'">
                <div class="card ">
                    <div class="card-header k">
                        Asuransi dan Layanan Kesehatan Telkomedika
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/kemahasiswaan/asuransi.png" alt="">
                    <div class="card-body l">
                        Layanan terkait pelaksanaan pengajuan klaim & asuransi kesehatan mahasiswa. 
                    </div>
                </div>
            </div>
        </div>

        <div class="row info mb-3">
            <h5 class="judul" style="display: flex;">
                <div class="brand-box"></div><span class="tulisann"> Informasi Kemahasiswaan</span>
            </h5>
            <div class="col-md-6">
                <p class="desk">Merupakan unit yang bertugas mengelola administrasi kemahasiswaan yang mencakup kegiatan layanan administrasi kemahasiswaan, pusat bahasa, dan perpustakaan. Informasi lengkap mengenai Unit Kemahasiswaan, silakan kunjungi:
                </p>
                <div class="row mb-3">
                    <div class="col-md-1">
                        <i class="fa-brands fa-instagram lgo"></i>
                    </div>
                    <div class="col-md-11">
                        <a class="links" href="https://www.instagram.com/kemahasiswaanitts/">kemahasiswaanitts</a>
                    </div>
                </div>
                <div class="row mt-3">
                    <div class="col-md-1">
                        <i class="fa-solid fa-globe lgo"></i>
                    </div>
                    <div class="col-md-11">
                        <a class="links" href="https://kemahasiswaan.ittelkom-sby.ac.id/">
                            https://kemahasiswaan.ittelkom-sby.ac.id/
                        </a>
                    </div>
                </div>
            </div>
            <div class="col-md-6">
                <img class="gambar" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/banner/device-kemahasiswaan.png" alt=""
                    width="650px">
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'KemahasiswaanView',
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
    font-size: 14px;
}
</style>