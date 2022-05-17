<template>
	<div class="mt-5">
		<!-- <b-button variant="success"> Texto </b-button>
		<b-button variant="info"> Texto </b-button>
		<b-button variant="danger"> Texto </b-button>
		<b-button variant="primary"> Texto </b-button>
		<b-button variant="warning"> Texto </b-button>

		<b-row class="mt-5">
			<b-col cols="12" md="4">
				<b-card
					title="Card Title"
					img-src="https://picsum.photos/300/300/?image=41"
					img-alt="Image"
					img-top
					tag="article"
					style="max-width: 20rem"
					class="mb-2"
				>
					<p>
						Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda
						maxime distinctio, reiciendis est minus optio praesentium, impedit
						maiores atque consectetur possimus laboriosam nam magnam a ipsa
						alias delectus. Debitis, voluptatem?
					</p>
					<b-button variant="dark" href="#"> Texto </b-button>
				</b-card>
			</b-col>
		</b-row> -->
		mostrar: {{ mostrar }}
		<br />
		estudios: {{ estudioss }}
		<div class="container row mr-6">
			<div class="card" style="width: 18rem">
				<img
					class="card-img-top img-fluid"
					src="../assets/negro.jpg"
					alt="Card image cap"
				/>
				<div class="text-center">
					<img
						class="img-fluid yoimagen rounded-circle img-thumbnail"
						src="../assets/io2022.jpeg"
						alt="Fabian :)"
						height="100px"
						width="100px"
					/>
				</div>
				<div class="card-body">
					<h5 class="card-title">Currículum</h5>
					<p class="card-text">
						Que hacer: botones a otras páginas con la información del curriculum
						o que cada boton active una tarjeta con las respectivas
						informaciones del curriculum, los botones tienen que hacer aparecer
						y desaparecer las nuevas tarjetas. O un conjunto de los 2 para
						"demostrar el uso de las dos opciones".
					</p>
					<div class="radio">
						Tarjetas:
						<label class="radio-inline mr-2">
							<input type="radio" v-model="mostrar" :value="true" />Sí
						</label>
						<label class="radio-inline">
							<input type="radio" v-model="mostrar" :value="false" />No
						</label>
					</div>
					<div v-show="mostrar">
						<a v-on:click="estudios(estudioss)" class="btn btn-primary mr-1"
							>Estudios</a
						>
						<a v-on:click="habilidades(habilidadess)" class="btn btn-info">Habilidades</a>
					</div>
				</div>
			</div>
			
				<div v-if="mostrar & estudioss === true" class="card" style="width: 18rem">
					<img
						class="card-img-top img-fluid"
						src="../assets/negro.jpg"
						alt="Card image cap"
					/>
					<div class="text-center">
						<img
							class="img-fluid yoimagen rounded-circle img-thumbnail"
							src="../assets/io2022.jpeg"
							alt="Fabian :)"
							height="100px"
							width="100px"
						/>
					</div>
					<div class="card-body">
						<h5 class="card-title">Currículum</h5>
						<p class="card-text">
							Que hacer: botones a otras páginas con la información del
							curriculum o que cada boton active una tarjeta con las respectivas
							informaciones del curriculum, los botones tienen que hacer
							aparecer y desaparecer las nuevas tarjetas. O un conjunto de los 2
							para "demostrar el uso de las dos opciones".
						</p>
						<a class="btn btn-primary mr-1">Grid</a>
						<a href="#" class="btn btn-info">Experiencia</a>
					</div>
				</div>
				<div v-if="mostrar & habilidadess === true" class="card" style="width: 18rem">
					<img
						class="card-img-top img-fluid"
						src="../assets/negro.jpg"
						alt="Card image cap"
					/>
					<div class="text-center">
						<img
							class="img-fluid yoimagen rounded-circle img-thumbnail"
							src="../assets/io2022.jpeg"
							alt="Fabian :)"
							height="100px"
							width="100px"
						/>
					</div>
					<div class="card-body">
						<h5 class="card-title">Currículum</h5>
						<p class="card-text">
							Que hacer: botones a otras páginas con la información del
							curriculum o que cada boton active una tarjeta con las respectivas
							informaciones del curriculum, los botones tienen que hacer
							aparecer y desaparecer las nuevas tarjetas. O un conjunto de los 2
							para "demostrar el uso de las dos opciones".
						</p>
						<a class="btn btn-primary mr-1">Grid</a>
						<a href="#" class="btn btn-info">Experiencia</a>
					</div>
				</div>
			</div>
		
	</div>
</template>

<script>
export default {
	name: "Cards",
	data() {
		return {
			mostrar: null,
			estudioss: false,
			habilidadess: false,
		};
	},
	methods: {
		estudios: function (event) {
			if (event === false) {
				this.estudioss = true;
			} else {
				this.estudioss = false;
			}
		},
		habilidades: function (event) {
			if (event === false) {
				this.habilidadess = true;
			} else {
				this.habilidadess = false;
			}
		},
	},
};
</script>
<style scoped>
.yoimagen {
	margin-top: -70px;
	border: -4px solid #ddd;
}
</style>
