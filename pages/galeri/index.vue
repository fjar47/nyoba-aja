<template>
  <div class="container-fluid">
    <div class="text-center judul pt-5">
      <h2 class="text-secondary pt-5">GALERI</h2>
      <h4 class="text-primary">SMKN 4 TASIKMALAYA</h4>
    </div>
    <div class="galeri d-flex justify-content-center">
      <div class="card m-5 shadow rounded-5" style="width: 80%">
        <div class="row p-4 m-3 d-flex justify-content-center">
          <div v-for="(foto, i) in galeri" :key="i" class="col-3 p-3">
            <img :src="foto.foto" class="cover" alt="" style="width: 80%;  object-fit: cover" />
          </div>
          <div v-for="(foto, i) in galeri" :key="i" class="col-3 p-4">
            <img :src="foto.foto" class="cover" alt="" style="width: 80%;  object-fit: cover" />
          </div>
        </div>
      </div>
    </div>
    </div>
</template>
<script setup>
useHead({ title: "Galeri" })

const supabase = useSupabaseClient()
const galeri = ref([])

const getGaleri = async () => {
  const { data, error } = await supabase
    .from('galeri')
    .select('foto')
  if (error) {
    console.error('Error fetching gallery:', error)
  } else {
    galeri.value = data
  }
}

onMounted(() => {
  getGaleri()
})
</script>

<style scoped>
img {
  height: 110px;
  margin-left: 10px;
}
@media (max-width: 768px) {
  img {
  height: 2rem;
  margin-left: 0.1rem;
}}
</style>
