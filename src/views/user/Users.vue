<template>
	<section>
		<h1>USUARIOS</h1>
		<hr />
<!-- Criando transicoes entre cada tela-->
		<!-- <transition mode="out-in"
		enter-active-class="elIn"
		leave-active-class="elOut"> -->
			<router-view />
		<!-- </transition> -->
		<button backBtn @click="goTo()">VOLTAR</button>
	</section>
</template>

<script>
export default {
	name: "Users",
	methods: {
		// A funcao goTo deve ser implementada como mixin
		goTo(params) {
			// ALGUMA MANEIRAS PARA REDIRECIONAR PARA UMA TELA
			// this.$router.push('/')
			// this.$router.push({path: '/'})

			//chama uma rota passando um paramentro
			// this.$router.push({path: `/newUser/${params}`})

			// Chama uma tela pelo nome da tela/componente
			this.$router.push({path: '/'})
		}

	}
}
</script>

<style scoped>
[backBtn] {
	background: rgb(72, 207, 207);
	color: rgb(214, 37, 185);
	width: 250px;
	height: 25px;
}

.elIn {
  transform: translate(0px, 0px);
  transition: box-shadow 2000ms ease;
}

.elIn:hover {
  box-shadow: inset 0px 200px 185px 0px rgba(35, 109, 173, 0.64);
}

.elOut {
  transform: translate(0px, 0px);
  transition: transform 1000ms ease-out;
}

.elOut:hover {
  transform: rotate(90deg) translate(200px, -200px);
}
</style>