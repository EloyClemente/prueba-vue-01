
<template>

    <div id="container_prueba">
        <h3 class="leccion-titulo" @click="miFuncion()">{{ titulo }}</h3>
    </div>
    
</template>




<script>
    export default {
        
        props: {
            titulo: {
                type: String,
                default: 'Titulo'
            },
            miFuncion: {
                type: Function
            },
            idContainer: String
        }
    }
</script>




<style>

</style>