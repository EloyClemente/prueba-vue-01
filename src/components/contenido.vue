
<template>

    <h3 class="leccion-titulo">{{ titulo }}</h3>
    
</template>




<script>
    export default {
        
        props: {
            titulo: {
                type: String,
                default: 'Titulo'
            }
        }
    }
</script>




<style>

</style>