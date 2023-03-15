<template>
    <div>
        <div class="row info mb-3">
            <h5 class="judul " style="display: flex;">
                <div class="brand-box"></div><span class="tulisann"> Layanan Logistik</span>
            </h5>
            <div class="col-md-4">
                <div class="justify-content-center py-auto">
                    <div class="list-group teks">
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi1' }" @click="viu = 'opsi1'"
                            aria-current="true">
                            <i class="fa-regular fa-square-check"></i> Peminjaman Asset
                        </a>
                        <a class="list-group-item py-3 px-4" :class="{ actives: viu === 'opsi2' }" @click="viu = 'opsi2'"><i
                                class="fa-regular fa-square-check"></i>
                            Pemeliharaan Asset Rusak / Hilang</a>
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi1" v-if="viu === 'opsi1'">
                <div class="card ">
                    <div class="card-header k ">
                        Peminjaman Asset
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/logistik/peminjaman.png" alt="">
                    <div class="card-body l">
                        Layanan peminjaman asset seperti ruangan kuliah, aula rapat, serta perlengkapan audio & video. 
                    </div>
                </div>
            </div>
            <div class="col-md-8" id="opsi2" v-if="viu === 'opsi2'">
                <div class="card ">
                    <div class="card-header k">
                        Pemeliharaan Asset Rusak / Hilang
                    </div>
                    <img class="foto card-img-top align-self-center"
                        src="https://ssc.ittelkom-sby.ac.id/assets-home/imgs/page/logistik/pemeliharaan.png" alt="">
                    <div class="card-body l">
                        Layanan pemeliharaan asset mengenai kelistrikan, air, gedung, audio & video yang rusak atau hilang. 
                    </div>
                </div>
            </div>
            
        </div>

        <div class="row info mb-3">
            <h5 class="judul" style="display: flex;">
                <div class="brand-box"></div><span class="tulisann"> Informasi Logistik</span>
            </h5>
            <div class="col-md-6">
                <p class="desk">Merupakan unit yang bertugas mengelola administrasi logistik yang mencakup kegiatan layanan administrasi logistik, pusat bahasa, dan perpustakaan. Informasi lengkap mengenai Unit Logistik, silakan kunjungi:
                </p>
                <div class="row mb-3">
                    <div class="col-md-1">
                        <i class="fa-brands fa-instagram lgo"></i>
                    </div>
                    <div class="col-md-11">
                        <a class="links" href="https://www.instagram.com/logistik.ittelkomsby/">logistik.ittelkomsby</a>
                    </div>
                </div>
                <div class="row mt-3">
                    <div class="col-md-1">
                        <i class="fa-solid fa-globe lgo"></i>
                    </div>
                    <div class="col-md-11">
                        <a class="links" href="https://logistik.ittelkom-sby.ac.id/">
                            https://logistik.ittelkom-sby.ac.id/
                        </a>
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
    name: 'LogistikView',
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