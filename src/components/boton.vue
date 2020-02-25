<template>
    <button class="boton" v-text="texto"></button>
</template>



<script>
    export default {
        data()
        {
            return{
                texto: 'Enviar'
            }
        }
    }
</script>




<style scoped>
    .boton{
        padding: 5px 10px;
        color: #fff;
        background-color: royalblue;
        border: 1px solid royalblue;
        border-radius: 3px;
        font-size: 18px;
        margin: 1px;
    }
</style>