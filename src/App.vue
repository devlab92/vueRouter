<template>
	<div id="app">
		<h1>APP</h1>
		<hr>
		<!-- O component MENU sera chamado pelo route-view abaixo que esta declarado no COMPONENTS do rota Users -->
		
			
		<router-view name="menu"/>
		
		<router-view/>

	</div>
</template>

<script>
import Menu from './components/Menu.vue'
export default {
	name: 'App',
	components: {
		Menu
		// HelloWorld
	}
}</script>
<style scoped>

</style>