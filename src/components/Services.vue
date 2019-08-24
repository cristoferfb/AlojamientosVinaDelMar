<template lang="pug">
	div
		v-container.text-center
			p.services-header.mb-0.pb-0 What we do
			p.services-body.mt-0.pt-0 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
		v-row
			v-col
				v-carousel(continuous).d-flex
					v-carousel-item.d-flex
						v-img(src="../assets/img1.jpg").d-flex
			v-col.pa-12
				img(src="../assets/start.png")
				p.services-subheader Brand Identity
				p.services-subbody Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
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
	}

	.services-subbody {
		font-size: 14px;
		font-weight: 400;
		font-family: "Roboto";
		color: #9299a5;
	}

	.services {

	}
</style>