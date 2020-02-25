<template>
	<div id="app" style="padding: 15px;">

		<h2>Temario</h2>
		<br>

		<Componente01/>
		<Componente02/>

		<Contenido 
			titulo="Desconexión del centro"
			idContainer="container_001"
			:miFuncion="function(){ prueba('container_prueba') }" 
		/> 

		<Contenido titulo="Autoimagen y supermodelo"/>
		<Contenido titulo="El centramiento" />

	</div>
</template>




<script>
	import Componente01 from './components/componente-01.vue'
	import Componente02 from './components/componente-02.vue'
	import Contenido from './components/contenido.vue'
	// import Leccion001 from './components/leccion-001.vue'
	// import Leccion002 from './components/leccion-002.vue'


	export default {
		name: 'App',
		components: {
			Componente01,
			Componente02,
			Contenido,
			// Leccion001
			// Leccion002
		},
		methods: {
			prueba: function(id)
			{
				let container = document.getElementById(id)
				console.log(container)
				container.style.border = "1px solid blue"
			}
		}
	}
</script>





<style>
  @import './assets/css/styles.css'
</style>
