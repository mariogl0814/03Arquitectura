<script setup>
    import { ref } from 'vue';

    const modelos = ref([
        {   
            tipo: 'basico', 
            heading: 'Modelo Básico',
            parrafo: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti, odit? Distinctio iure temporibus ab repellendus iste reiciendis accusantium nostrum, sit, cum accusamus omnis tempora facilis facere, pariatur ad repellat ex!',
            boton: 'Más Información'
        },
        {   
            tipo: 'premier', 
            heading: 'Modelo Premier',
            parrafo: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti, odit? Distinctio iure temporibus ab repellendus iste reiciendis accusantium nostrum, sit, cum accusamus omnis tempora facilis facere, pariatur ad repellat ex!',
            boton: 'Más Información'
        },
        {   
            tipo: 'elite', 
            heading: 'Modelo Elite',
            parrafo: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti, odit? Distinctio iure temporibus ab repellendus iste reiciendis accusantium nostrum, sit, cum accusamus omnis tempora facilis facere, pariatur ad repellat ex!',
            boton: 'Más Información'
        }
    ])
</script>
  
<template>
    <main class="contenedor mt-5">
        <h2 class="text-center">Nuestros modelos</h2>

        <div v-for="modelo in modelos" :key="modelo.tipo" :class="`modelo ${modelo.tipo}`">
            <div class="contenido-modelo">
                <h3>{{ modelo.heading }}</h3>
                <p>{{ modelo.parrafo }}</p>
                <a href="#" class="btn">{{ modelo.boton }}</a>
            </div>
        </div> <!--.modelo-->

    </main>

</template>
  
<style scoped>
  
</style>
  