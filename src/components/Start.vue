<template>
	<div class="hello">
		<h1>INICIO</h1>
		<router-link to="/users" active-class="active" exact>USUARIOS APP</router-link>
		<br>
		<router-link :to="{name: 'Alternative'}">Alternative</router-link>
	</div>
</template>

<script>
export default {
	name: 'Menu'

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
a {
	font-family: "Nunito";
	font-size: 14px;
	transition: all 0.3s;
}

a:hover {
	font-size: 16px;
	font-family: "Nunito-ExtraBold";
}

.active {
	font-size: 1.1em;
}
</style>
