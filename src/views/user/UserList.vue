<template>
	<section>
		<h1>Lista de Usuarios</h1>

		<ul>
			<router-link tag="li" :to="{name: 'DetailedUser', params: { id: 'um' }}">Usuario 1</router-link>
			<router-link tag="li" to="detailedUser/2">Usuario 2</router-link>
			<router-link tag="li" to="detailedUser/3">Usuario 3</router-link>
			<router-link tag="li" to="detailedUser/4">Usuario 4</router-link>
		</ul>
<hr>

<router-view/>

		
	</section>
</template>

<script>
export default {
	name: "UserList",
	methods: {
	
	}
}
</script>

<style scoped>
li:hover{
	cursor: pointer;
}
</style>