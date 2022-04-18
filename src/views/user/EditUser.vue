<template>
	<section>
		<h1>EDITAR USUARIO</h1>

		<h2> PARAMETRO: <strong>{{ id }}</strong></h2>
		<h3> Query name: {{ $route.query.name }}</h3>
		<h3> Query idade: {{ $route.query.idade }}</h3>

		<router-link tag="button" :to="`/deleteUser/${id}`">Deletar esse usuario!</router-link>
		<!-- Essa opcao abaixo chama a tela de deletar usuario pelo NOME da tela -->
		<router-link tag="button" :to="{ name: 'delUser', params: {id}, hash: '#hashId'}">delUser com HASH!</router-link>
		
	</section>
</template>

<script>
export default {
	name: "DeleteUser",
	props: ['id'],
	methods: {
	
	}
}
</script>

<style scoped>

</style>