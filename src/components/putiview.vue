<template>
    <div>
        <div class="row info mb-3">
            <h5 class="judul " style="display: flex;">
                <div class="brand-box"></div><span class="tulisann"> Layanan Puti</span>
            </h5>
            <div class="col-md-4">
                <div class="justify-content-center py-auto">
                    <div class="list-group teks">
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi1' }" @click="viu = 'opsi1'"
                            aria-current="true">
                            <i class="fa-regular fa-square-check"></i> Manajemen Akun
                        </a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi2' }" @click="viu = 'opsi2'"><i
                                class="fa-regular fa-square-check"></i>
                            Akses Internet</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi3' }" @click="viu = 'opsi3'"><i
                                class="fa-regular fa-square-check"></i>
                            Layanan Aplikasi</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi4' }" @click="viu = 'opsi4'"><i
                                class="fa-regular fa-square-check"></i>
                            Layanan Hosting</a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi5' }" @click="viu = 'opsi5'"><i
                                class="fa-regular fa-square-check"></i>
                            Pengembangan Aplikasi</a>
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi1" v-if="viu === 'opsi1'">
                <div class="card ">
                    <div class="card-header k ">
                        Manajemen Akun (iGracias, eLearning, WiFi)
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/puti/manajemen-akun.png" alt="">
                    <div class="card-body l">
                        Layanan untuk permintaan akun Email, iGracias, e-Learning, WiFi, Office365 untuk menunjang
                        keberlangsungan kegiatan akademik.
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi2" v-if="viu === 'opsi2'">
                <div class="card ">
                    <div class="card-header k">
                        Akses Internet
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/puti/internet.png" alt="">
                    <div class="card-body l">
                        Layanan untuk pengaduan mengenai akses internet yang putus nyambung (Blind Spot) dan login wifi
                        undefined, serta peminjaman Orbit atau kebutuhan internet untuk event
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi3" v-if="viu === 'opsi3'">
                <div class="card ">
                    <div class="card-header k">
                        Layanan Aplikasi
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/puti/layanan-aplikasi.png" alt="">
                    <div class="card-body l">
                        Layanan untuk mengatasi aplikasi (iGracias, Elearning dsb) yang terkena masalah seperti bug dan
                        error yang berdampak terhadap keberlangsungan kegiatan akademik. </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi4" v-if="viu === 'opsi4'">
                <div class="card ">
                    <div class="card-header k">
                        Layanan Hosting
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/puti/layanan-hosting.png" alt="">
                    <div class="card-body l">
                        Layanan untuk memenuhi permintaan domain dan VPS untuk keperluan hosting aplikasi atau website
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi5" v-if="viu === 'opsi5'">
                <div class="card ">
                    <div class="card-header k">
                        Pengembangan Aplikasi
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/puti/pengembangan-app.png" alt="">
                    <div class="card-body l">
                        Layanan pembuatan solusi sistem informasi untuk memenuhi kebutuhan proses bisnis.
                    </div>
                </div>
            </div>
        </div>

        <div class="row info mb-3">
            <h5 class="judul" style="display: flex;">
                <div class="brand-box"></div><span class="tulisann"> Informasi PuTi</span>
            </h5>
            <div class="col-md-6">
                <p class="desk">Merupakan unit yang bertugas mengelola administrasi puti yang mencakup kegiatan layanan
                    administrasi puti, pusat bahasa, dan perpustakaan. Informasi lengkap mengenai Unit PuTi, silakan
                    kunjungi:
                </p>
                <div class="row mb-3">
                    <div class="col-md-1">
                        <i class="fa-brands fa-instagram lgo"></i>
                    </div>
                    <div class="col-md-11">
                        <a class="links" href="https://www.instagram.com/puti.ittelkomsby/">puti.ittelkomsby</a>
                    </div>
                </div>
                <div class="row mt-3">
                    <div class="col-md-1">
                        <i class="fa-solid fa-globe lgo"></i>
                    </div>
                    <div class="col-md-11">
                        <a class="links" href="https://puti.ittelkom-sby.ac.id/">
                            https://puti.ittelkom-sby.ac.id/
                        </a>
                    </div>
                </div>
            </div>
            <div class="col-md-6">
                <img class="gambar" src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/banner/device-puti.png" alt=""
                    width="650px">
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'PutiView',
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