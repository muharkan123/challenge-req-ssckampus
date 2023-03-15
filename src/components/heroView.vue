<template>
    <div class="hero">
        <div class="row align-items-center mt-4">
            <!-- desktop -->
            <div class="col-lg-5 col-md-2  d-md-block d-none">
                <div class="ml-2 kolom">
                    <h1>
                        <span class="tulisann">S</span>tudent
                    </h1>
                    <h1>
                        <span class="tulisann">S</span>ervice
                    </h1>
                    <h1>
                        <span class="tulisann">C</span>enter
                    </h1>
                    <h6 class="tulis2">Datang, Buat Tiket, Proses</h6>
                    <button type="button" class="btn tombol">Lihat Layanan</button>
                </div>
            </div>

            <!-- mobile -->
            <!-- 
        <div class="col-lg-5 col-md-2 d-md-none d-sm-block">
            <div class="ml-2 align-items-center">
                <h1>
                    <span class="tulisann">S</span>tudent
                </h1>
                <h1>
                    <span class="tulisann">S</span>ervice
                </h1>
                <h1>
                    <span class="tulisann">C</span>enter
                </h1>
                <h6 class="tulis2">Datang, Buat Tiket, Proses</h6>
                <button type="button" class="btn tombol">Lihat Layanan</button>
            </div>
        </div> -->

            <!-- Desktop -->

            <div class="col-lg-7 col-md-2 d-md-block d-none">
                <img src="../assets/sschero.png" alt="" srcset="" width="640px">
            </div>

            <!-- Mobile -->

            <!-- <div class="d-md-none d-sm-block col-sm-2 col-md-2 mt-2">
            <img src="../assets/sschero.png" alt="" srcset="" width="420px">
        </div> -->

        </div>

        <div class="baris row mb-1 " style="margin-top:100px">
            <h5 class="judul"><i class="fa-solid fa-window-restore" style="color:rgb(170, 1, 1);"></i><span
                    class="tulisann"> Panduan</span> Pengajuan Layanan
            </h5>
            <div>
                <timelineHero />
            </div>
        </div>

        <div class="baris2 row ">
            <h5 class="judul"><i class="fa-solid fa-window-restore" style="color:rgb(170, 1, 1);"></i><span
                    class="tulisann"> Kategori</span> Layanan
            </h5>
            <div class="layanan">
                <div class="row mb-3 mt-3">
                    <div class="col-md-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan1'">
                                <lord-icon class="card-img-top align-self-center mt-2 ikon"
                                    src="https://cdn.lordicon.com/wxnxiano.json" trigger="morph"
                                    colors="primary:#911710,secondary:#121331" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title judul2">
                                        <h5 style="font-size: 17px">Akademik</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan2'">
                                <lord-icon class="card-img-top align-self-center mt-2"
                                    src="https://cdn.lordicon.com/qhgmphtg.json" trigger="hover"
                                    colors="primary:#121331,secondary:#911710" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title judul2">
                                        <h5 style="font-size: 17px">Puti</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan3'">
                                <lord-icon class="card-img-top align-self-center mt-2"
                                    src="https://cdn.lordicon.com/uukerzzv.json" trigger="hover"
                                    colors="primary:#121331,secondary:#911710" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title judul2">
                                        <h5 style="font-size: 17px">Kemahasiswaan</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan4'">
                                <lord-icon class="card-img-top align-self-center mt-2"
                                    src="https://cdn.lordicon.com/sbiheqdr.json" trigger="hover"
                                    colors="primary:#121331,secondary:#911710" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title judul2">
                                        <h5 style="font-size: 17px">Logistik</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3 mt-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan5'">
                                <lord-icon class="card-img-top align-self-center mt-2"
                                    src="https://cdn.lordicon.com/vaeagfzc.json" trigger="hover"
                                    colors="primary:#121331,secondary:#911710" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title judul2">
                                        <h5 style="font-size: 17px">Keuangan</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3 mt-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan6'">
                                <lord-icon class="card-img-top align-self-center mt-2"
                                    src="https://cdn.lordicon.com/gdjyhaga.json" trigger="morph"
                                    colors="primary:#121331,secondary:#911710" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title">
                                        <h5 style="font-size: 17px">Pusat Bahasa & Perpustakaan</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3 mt-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan7'">
                                <lord-icon class="card-img-top align-self-center mt-2"
                                    src="https://cdn.lordicon.com/nobciafz.json" trigger="hover"
                                    colors="primary:#121331,secondary:#911710" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title judul2">
                                        <h5 style="font-size: 17px">FTIB</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                    <div class="col-md-3 mt-3">
                        <div class="card text-center kartu">
                            <a class="judul2" @click="tampil = 'layanan8'">
                                <lord-icon class="card-img-top align-self-center mt-2" src="https://cdn.lordicon.com/ckuogwdx.json" trigger="hover"
                                    colors="primary:#121331,secondary:#911710" style="width:90px;height:90px">
                                </lord-icon>
                                <div class="card-body">
                                    <div class="card-title judul2">
                                        <h5 style="font-size: 17px">FTEIC</h5>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </div>
                </div>
                <div class="row mb-3 mt-3">
                    <div class="row" id="layanan1" v-if="tampil === 'layanan1'">
                        <AkademikView />
                    </div>
                    <div class="row" id="layanan2" v-if="tampil === 'layanan2'">
                        <PutiView />
                    </div>
                    <div class="row" id="layanan3" v-if="tampil === 'layanan3'">
                        <KemahasiswaanView />
                    </div>
                    <div class="row" id="layanan4" v-if="tampil === 'layanan4'">
                        <LogistikView />
                    </div>
                    <div class="row" id="layanan5" v-if="tampil === 'layanan5'">
                        <KeuanganView />
                    </div>
                    <div class="row" id="layanan6" v-if="tampil === 'layanan6'">
                        <PerpusView />
                    </div>
                    <div class="row" id="layanan7" v-if="tampil === 'layanan7'">
                        <FtibView />
                    </div>
                    <div class="row" id="layanan8" v-if="tampil === 'layanan8'">
                        <FteicView />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import timelineHero from './timelineHero.vue'
import AkademikView from './akademikview.vue'
import PutiView from './putiview.vue'
import PerpusView from './perpusview.vue'
import KemahasiswaanView from './kemahasiswaanview.vue'
import LogistikView from './logistikview.vue'
import KeuanganView from './keuanganview.vue'
import FteicView from './fteicview.vue'
import FtibView from './ftibview.vue'
export default {
    name: 'heroView',
    components: {
        timelineHero,
        AkademikView,
        PutiView,
        KemahasiswaanView,
        LogistikView,
        KeuanganView,
        PerpusView,
        FtibView,
        FteicView
    },
    data() {
        return {
            tampil: 'layanan1'
        }
    }

}
</script>



<style scoped>
.active {
    background-color: rgb(170, 1, 1);
    color: white;
}

.ikon:active {
    color: white;
}

.kartu:active {
    background-color: rgb(170, 1, 1);
    color: white;
}

a:hover {
    color: rgb(170, 1, 1);
    text-decoration: none;
}

a:active {
    color: white;
}

a {
    color: rgb(46, 46, 46);
    outline: none;
}

.kolom {
    padding-left: 50px;
    padding-top: 40px;
}

.baris2 {
    margin-top: 120px;
}

.baris2 {
    margin-top: 70px;
}

.tulisann {
    color: rgb(170, 1, 1);
}

.judul {
    font-family: 'League Spartan', sans-serif;
    font-weight: 600;
}

.judul2 {
    font-family: 'League Spartan', sans-serif;
    font-weight: 700;
    font-size: 16px;
    text-decoration: none;
}


.tombol {
    background-color: rgb(170, 1, 1);
    color: white;
    font-family: 'League Spartan', sans-serif;
    font-weight: 600;
    font-size: 13px;
    width: 150px;
    height: 45px;
    border-radius: 10px;
}

.tombol:hover {
    background-color: rgb(218, 0, 0);
}

.tombol:active {
    border-color: rgb(218, 0, 0);
    color: white;
}

.tulis2 {
    color: rgb(85, 85, 85);
}
</style>