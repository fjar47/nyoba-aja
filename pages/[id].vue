<template>
    <div class="container-fluid">
        <div class="foto p-5  text-center">
            <img :src="berita.foto" alt="foto" style="width:80%;" v-if="berita" />
        </div>
        <div class="tanggal px-5 mx-5">
        <p class="px-5 mx-5">{{ berita.tanggal }}</p>
        </div>
        <div class="content px-5 mx-5">
            <h3 class="pb-5 px-5 mx-5">
            {{ berita.judul }}
            </h3>
        </div>
        <div class="content px-5 mx-5">
        <p class="px-5 pb-5 mx-5">
        {{ berita.isi }}
        </p>
        </div>
    </div>
</template>

<script setup>
useHead({ title: "berita" })
const supabase = useSupabaseClient();
const berita = ref({});
const route = useRoute();

const getBerita = async () => {
    const { data, error } = await supabase
        .from('berita')
        .select(`*`)
        .eq('id', route.params.id);

    if (data && data.length > 0) {
        berita.value = data[0];
    }
};

onMounted(() => {
    getBerita();
});
</script>
