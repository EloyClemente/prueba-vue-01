
<template>
    <div id="container_002" class="leccion-container" v-on:click="altura">

        <h3 class="leccion-titulo">Aforismos de Antonio Blay</h3>

        <div id="contenido_002" class="leccion-contenido" v-if="mostrar">
            <p>Nada de lo que se diga de mí, lo Soy.</p>
            <p>Mirar con interés para ver y comprender.</p>
            <p>Nadie puede manejar bien aquello con lo que está identificado.</p>
            <p>Mientras vivas en lo que sientes, mal. Vive en lo que Eres detrás de lo que sientes.</p>
            <p>Una clave importante: no vivamos el cómo soy; busquemos qué soy; y después, quién soy.</p>
            <p>Yo soy más yo, allí donde soy Inteligencia, soy Voluntad y soy Amor. Y eso que soy, lo soy como un punto focal de algo más grande.</p>
            <p>En la medida que descubro lo que Soy, veo también lo que no soy. Entonces adquiero poder sobre esto que no soy el personaje o una serie de ellos.</p>
            <p>Tú ya eres la Realidad que eres. Tú ya estás realizado. El problema está en que no te lo crees, pues tú crees ser algo o alguien: Margarita, José, etc.</p>
        </div>
        
    </div>
</template>




<script>
    export default {

        name: 'componente-02',

        data()
        {
            return {
                mostrar: false
            }
        },

        methods: {

            altura()
            {
                var container = document.getElementById('container_002')
                var that = this


                if(this.mostrar == false)
                {
                    this.mostrar = !this.mostrar

                    setTimeout(function()
                    {
                        var contenido = document.getElementById('contenido_002')
                        container.style.height = contenido.offsetHeight + 30 + 'px';
                    }, 10)
                }
                else
                {
                    container.style.height = '30px';

                    setTimeout(function()
                    {
                        that.mostrar = !that.mostrar
                    }, 300)
                }    
            }
        }
    }
</script>




<style>

</style>