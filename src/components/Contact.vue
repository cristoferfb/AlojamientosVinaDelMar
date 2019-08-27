<template lang="pug">
	v-container(id="contact").text-center
		p(:class="{'services-header-mobile': $vuetify.breakpoint.mdAndDown}").services-header Contacto
		p.body-contact +569 54959743
		p(:class="{'mobile-contact': $vuetify.	breakpoint.mdAndDown}").body-contact contacto@alojamientosvinadelmar.cl
		v-row
			v-col
				v-btn(
					text
					href="https://www.facebook.com/Alojamientos-Viña-del-Mar-107616807270388"
					target="_blank"
				)
					v-icon(x-large) mdi-facebook-box
			v-col
				v-btn(
					text
					href="https://www.instagram.com/alojamientosvina/"
					target="_blank"
				)
					v-icon(x-large) mdi-instagram

</template>

<style type="text/css">
	.body-contact {
		color: #aab3c2;
		font-size: 40px;
	}

	.mobile-contact {
		font-size: 20px;
	}
</style>