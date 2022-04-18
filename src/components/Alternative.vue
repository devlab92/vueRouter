<template>
  <div class="hello">
    <h1>Alternative <strong>OPTIONS</strong></h1>
	<!-- essa rota possui um redirecionamento. Quando ela eh acessa automaticamente voce eh redirecionado para o Start -->
	<router-link to="/redirect"><h3>/redirect</h3></router-link>
	
   
  </div>
</template>

<script>
export default {
  name: 'Alternative'

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
a{
	font-family: 'Nunito';
	font-size: 14px;
	transition: all 0.3s;
}

a:hover{
	font-size: 16px;
	font-family: 'Nunito-ExtraBold';
}

.active{
	font-size: 1.1em;
}
</style>
