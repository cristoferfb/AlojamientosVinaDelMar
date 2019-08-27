<template lang="pug">
    v-container(fluid)
        v-row(dense)
            v-col(
                :class="{'padding-header-desktop': $vuetify.breakpoint.lgAndUp, 'text-center': $vuetify.breakpoint.smAndDown}"
                :style="{marginTop: ($vuetify.breakpoint.mdAndUp) ? windowHeight/2-230 + 'px' : 100 + 'px'}"
                lg="7" md="9" sm="12"
            )
                p.my-subheader ALOJAMIENTOS VIÑA DEL MAR
                p(:class="{'header-desktop mt-n10': $vuetify.breakpoint.mdAndUp, 'header-mobile mt-n6': $vuetify.breakpoint.smAndDown}").header.d-none.d-md-flex
                    span(style="z-index:2") Cuartos amoblados&nbsp;
                    span(style="z-index:2").redheader en
                p(:class="{'header-desktop mt-n12': $vuetify.breakpoint.mdAndUp, 'header-mobile mt-n7': $vuetify.breakpoint.smAndDown}").header.d-none.d-md-flex
                    span(style="z-index:2").redheader pleno centro&nbsp;
                    span(style="z-index:2") de viña
                p.header.header-mobile.d-md-none Cuartos amoblados en pleno centro de Viña
                p.body.d-none.d-md-flex Alojamiento excelentemente ubicado en pleno centro de Viña a pasos de locomocion y puntos de interes relevantes de la ciudad, habitaciones equipadas, tv cable, wifi, agua caliente y mas.
                v-btn(color="error" href="tel:56954959743")
                    v-icon() mdi-phone
                    span Llamar
            v-col(lg="5" md="3").pr-0.d-none.d-md-flex
                img(src="../assets/image.png" contain).ml-auto.d-flex
</template>

<script>
export default {
    data: () => ({
        windowHeight: window.innerHeight,
    })
}
</script>


<style>
    .padding-header-desktop {
        padding-left: 175px !important;
    }

    .my-subheader {
        font-size: 16px;
        color: #3eb3e5;
        font-family: "Roboto";
        margin-bottom: 10px;
    }

    .header {
        font-family: "Playfair Display";
        font-weight: 400;
        color: #535b6c;
    }

    .header-desktop {
        font-size: 80px;
        z-index: 2;
        display: flex;
        white-space: nowrap;
    }

    .header-mobile {
        font-size: 37px;
    }

    .redheader {
        color: #FE6B6F;
        font-weight: bold;
    }

    .body {
        display: flex;
        color: #aab3c2;
        font-family: "Roboto";
        margin-top: -5px;
    }
</style>