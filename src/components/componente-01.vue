
<template>
    <div id="container_001" class="leccion-container" v-on:click="altura">

        <h3 class="leccion-titulo">Aforismos de Gurdjieff</h3>

        <div id="contenido_001" class="leccion-contenido" v-if="mostrar">
            <p>Sólo puede ser justo quien es capaz de ponerse en el lugar de otros.</p>
            <p>Al hombre le es dado un número determinado de experiencias; al economizarlas, prolonga su vida.</p>
            <p>El razonamiento activo se aprende con la práctica; debería ser practicado durante mucho tiempo y de muchas maneras variadas.</p>
            <p>El amor propio es señal de una elevada opinión de uno mismo. Si un hombre tiene amor propio, esto demuestra lo que vale.</p>
            <p>La gente no tiene idea de hasta qué punto es arrastrada por el miedo. Este miedo no es fácilmente definible. Hay momentos en que este miedo se vuelve casi una obsesión.</p>
            <p>La constante conciencia de la inevitabilidad de la muerte es el único medio para adquirir la urgencia para redefinir al hombre.</p>
        </div>
        
    </div>
</template>




<script>
    export default {

        name: 'componente-01',

        data()
        {
            return {
                mostrar: false
            }
        },

        methods: {

            altura()
            {
                var container = document.getElementById('container_001')
                var that = this


                if(this.mostrar == false)
                {
                    this.mostrar = !this.mostrar

                    setTimeout(function()
                    {
                        var contenido = document.getElementById('contenido_001')
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