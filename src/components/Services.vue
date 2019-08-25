<template lang="pug">
	div(id="services")
		v-container.text-center
			p.services-header.mb-0.pb-0 Habitaciones
			p.services-body.ma-0.pa-0 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
			p.services-body et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
		v-row
			v-col(cols="12" lg="6").pb-0
				v-card(flat).pa-12.pb-0
					v-carousel(hide-delimiters )
						v-carousel-item(v-for="n in 3" :key="n")
							v-img(:src="'/galery/img'+n+'.jpg'" contain)
			v-col(cols="12" lg="4" style="z-index: 10" :class="{'pt-0': $vuetify.breakpoint.mdAndDown}").pa-12
				v-row
					v-col( cols="12" md="6" lg="12")
						img(src="../assets/start.png")
						p.services-subheader Brand Identity
						p.services-subbody Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
					v-col( cols="12" md="6" lg="12")
						img(src="../assets/figure.png")
						p.services-subheader Design
						p.services-subbody Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
						
</template>

<style>
	.services-header {
		color: #535b6c;
		font-family: "Playfair Display";
		font-size: 80px;
		font-weight: 400;
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
		z-index: 500 !important;
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