<template>
	<section>
		<h1>DELETAR USUARIO</h1>

		<h2> PARAMETRO: <strong>{{ id }}</strong></h2>
		
		<div id="hashId">
			<p>Estou sendo ancorado</p>
		</div>
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
#hashId{
	margin-top: 1000px;
}
</style>