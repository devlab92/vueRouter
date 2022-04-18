<template>
	<section>
		<h1>DETALHES DO USUARIO USUARIO {{ id }}</h1>
		<!-- Nessa router-link esta sendo chamado a tela pelo NAME, passando o ID como PARAMETROS na URL e enviando algumas infos via QUERY -->
		<router-link tag="button" :to="{
			name: 'EditUser', 
			params: { id }, 
			query: {idade: '25', name: 'Ricardo'}
		}">EDITAR USUARIO {{id}}</router-link>
	</section>
</template>

<script>
export default {
	name: "DetailedUser",
	props: ['id'],
	methods: {
		goTo(params) {
			this.$router.push({path: '/'})
		}
	}
}
</script>

<style scoped>

</style>