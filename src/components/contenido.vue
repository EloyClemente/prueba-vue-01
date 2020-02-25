
<template>

    <h3 class="leccion-titulo" @click="miFuncion()">{{ titulo }}</h3>
    
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
            }
        }
    }
</script>




<style>

</style>