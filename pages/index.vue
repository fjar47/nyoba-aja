<template>
  <div class="container-fluid">
    <img src="../assets/home.jpg" alt="" style="width: 100%" />
    <div class="berita">
      <h1 class="text-primary d-flex justify-content-center mt-5">BERITA</h1>
      <h4 class="text-secondary d-flex justify-content-center mb-5">
        SMKN 4 TASIKMALAYA
      </h4>
      <div class="content d-flex justify-content-center">
        <div class="row p-5">
          <div v-for="(foto, i) in berita" :key="i" class="col-3  p-3">
            <nuxt-link :to="`/${foto.id}`">
              <div class="card" style="height: 100%;">
                <img :src="foto.foto" class="img-fluid " alt="" />
                <h6 class="judul-berita text-center p-2">{{ foto.judul }}</h6>
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="sambutan p-3 d-flex justify-content-center">
      <div class="card p-5 rounded-5 shadow" style="width: 80%;">
        <div class="row g-4 p-2">
          <div class=" col-5 ">
            <img src="../assets/kepala.png" alt="" class="img-fluid rounded-5" />
          </div>
          <div class="col-7">
            <div class="judul-sambutan mb-3">
              <h2 class="text-primary">SAMBUTAN</h2>
              <h4 class="text-secondary">KEPALA SMKN 4 TASIKAMALAYA</h4>
            </div>
            <div class="content-s">
              <p>
              ASSALAMUALAIKUM, WR. WB.
                Selamat datang di SMKN 4 Tasikmalaya. Segala puji dan syukur kita panjatkan kehadirat Allah SWT,
                semoga kita semua ada dalam lindungan-Nya. Dan atas perkenan-Nya pula kami dapat menghadirkan
                website SMK Negeri 4 Tasikmalaya ini. Kami berharap dengan adanya website di SMK Negeri 4
                Tasikmalaya ini para pengunjung dapat mengenal lebih jauh tentang sekolah kami sehingga dapat
                mempererat tali silaturrahmi antara sekolah dengan masyarakat demi kemajuan kita bersama. Tiada
                gading yang tak retak, website kami ini masih dalam proses pengembangan, masih banyak kekurangan
                yang harus kami perbaiki. Kritik dan sarannya yang membangun sangat kami harapkan untuk
                pengembangan ke depan.
                Akhirnya, saya mengucapkan terimakasih yang sebesar-besarnya kepada semua pihak yang tidak dapat
                disebutkan satu segala bantuan dan persatu atas fasilitasnya yang telah diberikan semoga semua
                yang kita lakukan bermanfaat bagi masyarakat. Wassalamu'alaikum Warahmatullahi Wabarakatuh.

              </p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="data-sw rounded-4 p-5 my-2">
      <div class="judul text-center">
        <h1 class="text-primary">DATA SISWA DAN GURU</h1>
        <h4 class="text-secondary mb-5">
          SMKN 4 TASIKMALAYA
        </h4>
      </div>
      <div class="content-d p-5">
        <div class="row">

          <div class="col-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2">
                <div class="col-lg-3">
                  <img src="../assets/smktp.jpg" class="card-img-top rounded-2" alt="">
                </div>
                <div class="col-lg-4 text-center">
                  <h1>1400</h1>
                </div>
                <div class="col-lg-5 text-center">
                  <h1>SISWA</h1>
                </div>
              </div>
            </div>
          </div>
          <div class="col-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2">
                <div class="col-lg-3 ">
                  <img src="../assets/smktp.jpg" class="card-img-top rounded-2" alt="">
                </div>
                <div class="col-lg-4 text-center">
                  <h1>1400</h1>
                </div>
                <div class="col-lg-5 text-center">
                  <h1>SISWA</h1>
                </div>
              </div>
            </div>
          </div>
          <div class="col-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2 text-center">
                <div class="col-lg-3">
                  <img src="../assets/smktp.jpg" class="card-img-top rounded-2" alt="">
                </div>
                <div class="col-lg-4 text-center">
                  <h1>1400</h1>
                </div>
                <div class="col-lg-5 text-center">
                  <h1>SISWA</h1>
                </div>
              </div>
            </div>
          </div>
          <div class="col-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2">
                <div class="col-lg-3">
                  <img src="../assets/smktp.jpg" class="card-img-top rounded-2" alt="">
                </div>
                <div class="col-lg-4 text-center">
                  <h1>1400</h1>
                </div>
                <div class="col-lg-5 text-center">
                  <h1>SISWA</h1>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="judul ">
      <h1 class="text-center text-primary ">PROGRAM KEAHLIAN</h1>
      <h4 class="text-secondary text-center">
        SMKN 4 TASIKMALAYA
      </h4>
    </div>
    <div class="jurusan">
      <img src="../assets/jurusan.jpg" alt="" width="100%" />
    </div>
    <div class="patner">
      <div class="judul-patner">
        <h1 class="text-center text-primary">MITRA INDUSTRI</h1>
        <h4 class="text-secondary text-center">
          SMKN 4 TASIKMALAYA
        </h4>
      </div>
      <div class="scroll-container m-5">
        <div class="scroll-content">
          <div class="img p-5"><img src="../assets/perusahaan/agate.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/ahm.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/inovindo.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/semesta.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/skyline.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/cikara.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/agate.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/ahm.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/inovindo.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/semesta.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/skyline.png" alt=""></div>
          <div class="img p-5"><img src="../assets/perusahaan/cikara.png" alt=""></div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.scroll-container {
  overflow: hidden;
  white-space: nowrap;
  position: relative;
  height: 250px;
}

.scroll-content {
  display: flex;
  animation: scroll 5s linear infinite;
}

.scroll-content .img {
  flex: none;
  margin-right: 20px;
}

.scroll-content .img img {
  height: 200px;
  width: auto;
}

.card-img-top {
  width: 100%;
  height: auto;
}



.judul-sambutan h2 {
  font-size: 2rem;
}

.judul-sambutan h4 {
  font-size: 1.25rem;
}

.content-s p {
  font-size: 1rem;
}

.img-fluid {
  width: 100%;
  height: auto;
}


@keyframes scroll {
  0% {
    transform: translateX(0);
  }

  100% {
    transform: translateX(-100%);
  }
}



.img {
  flex: 0 0 auto;
}

@media (max-width: 768px) {
  .scroll-content .img img {
    height: 50px;
  }

  .scroll-content .img {
    flex: none;
    margin-right: 2px;
  }

  .judul-sambutan h2 {
    font-size: 1.5rem;
  }

  .judul-sambutan h4 {
    font-size: 1.1rem;
  }

  .content-s p {
    font-size: 0.9rem;
  }


  .scroll-content .img {
    flex: none;
    margin-right: 1px;
  }

  .data-sw .card {
    padding: 1rem;
  }

  .data-sw .row {
    margin-bottom: 1.5rem;
  }

  .data-sw .col-6 {
    padding: 0.5rem;
  }

  .data-sw h1 {
    font-size: 1.5rem;
  }

  .data-sw h4 {
    font-size: 1rem;
  }

  .data-sw .row .col-6 h1 {
    font-size: 0.5rem;
  }

  .row .col-3 .judul-berita {
    font-size: 0.2rem;
  }
  h1 {
    font-size: 1rem;
  }
.judul h1 {
    font-size: 1rem;
  }
h2{
    font-size: 0.8rem;
  }
h3{
    font-size: 0.6rem;
  }
  h4 {
    font-size: 0.4rem;
  }
.judul h4 {
    font-size: 0.4rem;
  }
  .judul-sambutan h2{
    font-size: 0.8rem;
  }
  .judul-sambutan h4{
    font-size: 0.4rem;
  }
  .content-s p{
    font-size: 0.1rem;
  }
  .sambutan img{
    width:40px;
  }

  @keyframes scroll {
    0% {
      transform: translateX(0);
    }

    100% {
      transform: translateX(-300%);
    }
  }
}
</style>
<script setup>
useHead({ title: "Home" })
const supabase = useSupabaseClient()
const berita = ref([])

const getBerita = async () => {
  const { data, error } = await supabase
    .from('berita')
    .select('*')
  if (error) {
    console.error('Error Berita:', error)
  } else {
    berita.value = data
  }
}

onMounted(() => {
  getBerita()
})
</script>
<style scoped>
* {
  text-decoration: none;
}

.judul-berita {
  color: black;
  position: sticky;

}
</style>