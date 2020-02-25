<template>
	<div id="app" style="padding: 15px;">

		<h2>Temario</h2>
		<br>

		<Componente01/>
		<Componente02/>

		<Contenido titulo="Desconexión del centro"/>
		<Contenido titulo="Autoimagen y supermodelo"/>
		<Contenido titulo="El centramiento"/>
		<Contenido/>

	</div>
</template>




<script>
	import Componente01 from './components/componente-01.vue'
	import Componente02 from './components/componente-02.vue'
	import Contenido from './components/contenido.vue'


	export default {
		name: 'App',
		components: {
			Componente01,
			Componente02,
			Contenido
		}
	}
</script>





<style>
  @import './assets/css/styles.css'
</style>
