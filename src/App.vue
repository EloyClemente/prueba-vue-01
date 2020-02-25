<template>
	<div id="app" style="padding: 15px;">

		<h2>Temario</h2>
		<br>

		<Componente01></Componente01>
		<Componente02></Componente02>		

	</div>
</template>




<script>
	import Componente01 from './components/componente-01.vue'
	import Componente02 from './components/componente-02.vue'


	export default {
		name: 'App',
		components: {
			Componente01,
			Componente02,
		}
	}
</script>





<style>
  @import './assets/css/styles.css'
</style>
