<template>
    <div class="kaki">
        <div class="futer ">
            <footer class="pt-md-5 pb-4 container">
                <div class="row">
                    <div class="col-5 col-md">
                        <h2>Student Service Center</h2>
                        <h6 style="color: grey">Contact</h6>
                        <p><strong>Address : </strong>Jl. Ketintang No.156, Gayungan, Surabaya, Jawa Timur 60231 </p>
                        <p><strong>Phone : </strong>(+6231) 8280800 </p>
                        <p><strong>Email : </strong>humas@ittelkom-sby.ac.id </p>
                    </div>
                    <div class="col-4 col-md">
                        <h4 style="padding-top:20px; font-size:18px;">Aplikasi Student Service Center</h4>
                        <p class="desc">Ditunjukkan untuk mempermudah perangkat kerja serta mahasiswa
                            Institut Teknologi Telkom Surabaya untuk melakukan pelaporan pemintaan bantuan, demi terciptanya
                            lingkungan kerja serta perkuliahan yang lebih baik dan efisien. </p>
                    </div>
                    <div class="col-3 ra pl-2">
                        <h4 style="padding-top:20px; font-size:18px;">My Account</h4>
                        <ul class="lis">
                            <li><a class="baris" href="#">My History</a>
                            </li>
                            <li><a href="#" class="baris">Services List</a>
                            </li>
                            <li><a href="#" class="baris">Sign Out</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </footer>

        </div>
        <div class="container">
            <footer class="d-flex flex-wrap justify-content-between align-items-center py-3">
                <p class="col-md-4 mb-0 text-muted" style="font-size: 13px">&copy; 2023, <strong style="color: rgb(170, 1, 1);">IT Telkom Surabaya</strong> Student Service Center</p>

                <ul class="nav col-md-4 justify-content-end align-items-center">
                    <p class="align-items-center my-auto justify-content-center"><strong>IT Telkom Surabaya</strong> All Right Reserved</p>
                </ul>
            </footer>
        </div>
    </div>
</template>

<script>
export default {
    name: 'footerView'
}
</script>

<style scoped>
.futer {
    background-color: rgb(46, 46, 46);
    color: white;
}

.baris {
    text-decoration: none;
    color: white;
    margin-top: 20px;
    margin-bottom: 20px;
}

li{
    margin: 10px 0;
}

.baris:hover {
    color: rgb(196, 0, 0);
    transform: translate(10px);
}

ul.lis {
    list-style-type: none;
}

.lis {
    margin: 0;
    padding: 0;
}

.ra {

    float: left;
}

.desc {
    color: gray;
    font-size: 16px;
    font-style: italic;
    line-height: 20px;
}</style>