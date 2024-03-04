<script setup>
    import {ref} from 'vue'

    import imagen_1 from "../assets/img/imagen_1.jpg";
    import imagen_2 from "../assets/img/imagen_2.jpg";
    import imagen_3 from "../assets/img/imagen_3.jpg";
    import imagen_4 from "../assets/img/imagen_4.jpg";
    import imagen_5 from "../assets/img/imagen_5.jpg";
    import imagen_6 from "../assets/img/imagen_6.jpg";
    import imagen_7 from "../assets/img/imagen_7.jpg";

    const imagenes = ref([
        { rutaImagen: imagen_1 },
        { rutaImagen: imagen_2 },
        { rutaImagen: imagen_3 },
        { rutaImagen: imagen_4 },
        { rutaImagen: imagen_5 },
        { rutaImagen: imagen_6 },
        { rutaImagen: imagen_7 },
    ])
</script>
  
<template>
    <section class="contenedor mt-5">
        <h2 class="text-center">Galería</h2>

        <div class="galeria">

            <div v-for="imagen in imagenes" :key="imagen.rutaImagen" class="imagen">
                <img :src="imagen.rutaImagen" alt="imagen galeria">
            </div>

        </div>
    </section>
</template>
  
<style scoped>
  
</style>
  