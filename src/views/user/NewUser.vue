<template>
	<section>
		<h1>NOVO USUARIO</h1>

		<label>NOME DO USUARIo</label>
		<input type="text" placeholder="Ex: Jao">
	</section>
</template>

<script>
export default {
	name: "NewUser",

	// AQUI VEMOS COMO CHAMAR E ATUALIZAR UMA ROTA QUE ESPERA PARAMETROS
	// data() {
	// 	return {
	// 		id: this.$route.params.id,
	// 	}
	// },
	// watch: {
	// 	// monitorar o route e usar TO e FROM para atualizar as variaveis quan houver mudancas de tela
	// 	//FROM guarda valor antigo
	// 	//TO guarda o valor novo
	// 	$route(to, from){
	// 		//console.log('TO: ', to,' -  FROM: ', from)
	// 		this.id = to.params.id
	// 	}
	// },
	// AQUI FAREMOS O MESMO, MAS DE FORMA MODERNA E COM MENOS CODIGO
	// EH NECESSARIO FAZER A IMPLEMENTACAO NO AQRUIVO ROUTER.JS INSERINDO UMA CHAVE 'PROPS' RECEBENDO VALOR TRUE
	// e assim nao eh necessario fazer nada para monitorar as atulizacoes das variaveis
	props: ['id'],
	methods: {
		// A funcao goTo deve ser implementada como mixin
		goTo(params){
			// this.$router.push('/')
			this.$router.push({path: '/'})

			//chama uma rota passando um paramentro
			// this.$router.push({path: `/newUser/${params}`})
		}
	
	}
}
</script>

<style scoped>

</style>