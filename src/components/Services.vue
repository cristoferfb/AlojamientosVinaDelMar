<template lang="pug">
	div(id="services")
		v-container.text-center
			p(:class="{'services-header-mobile': $vuetify.breakpoint.mdAndDown}").services-header.mb-0.pb-0 Habitaciones
		v-row(no-gutters)
			v-col(cols="12" lg="6" :class="{'pa-0': $vuetify.breakpoint.mdAndDown, 'pa-12': $vuetify.breakpoint.lgAndUp}")
				v-card(flat)
					v-carousel(hide-delimiters  height="auto")
						v-carousel-item(v-for="n in 14" :key="n")
							v-img(:src="'/galery/img'+n+'.jpg'")
			v-col(
				cols="12"
				lg="4"
				style="z-index: 10"
			).pa-5
				v-row(no-gutters)
					v-col(cols="12" md="6" lg="12")
						img(src="../assets/start.png")
						p.services-subheader Caracteristicas
						p.services-subbody Todas las habitaciones cuentan con su cama de dos plazas, mesa de noche, television con cable y armario, tambien tenemos disponible habitaciones con 2 camas y nuestra suite con baño privado.
					v-col(cols="12" md="6" lg="12")
						img(src="../assets/figure.png")
						p.services-subheader Ademas
						p.services-subbody Dispones de cocina completamente equipada y baños de uso compartido con agua caliente. Wi-Fi Incluido. 
						
</template>

<style>
	.services-header {
		color: #535b6c;
		font-family: "Playfair Display";
		font-weight: 400;
		font-size: 80px;
	}

	.services-header-mobile {
		font-size: 40px;
		margin-top: 30px;
	}

	.services-body {
		font-size: 16px;
		font-weight: 400;
		font-family: "Roboto";
		color: #aab3c2;
	}

	.services-subheader {
		color: #535b6c;
		font-family: "Playfair Display";
		font-size: 40px;
		font-weight: 400;
	}

	.services-subbody {
		font-size: 14px;
		font-weight: 400;
		font-family: "Roboto";
		color: #9299a5;
	}

	.custom-carousel {
		padding-left: 135px;
		padding-right: 135px;
		margin-top: 120px;
	}
</style>