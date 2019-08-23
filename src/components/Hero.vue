<template lang="pug">
    v-container.pa-0.ma-0
        v-row
            v-col(:class="{'margin-header-desktop': $vuetify.breakpoint.mdAndUp}" :style="{marginTop: windowHeight/2-230 + 'px'}" )
                p.my-subheader ALOJAMIENTOS VIÑA DEL MAR
                p(:class="{'header-desktop mt-n10': $vuetify.breakpoint.mdAndUp, 'header-mobile mt-n5': $vuetify.breakpoint.xsOnly}")
                    span Cuartos amoblados&nbsp;
                    span.redheader en
                p(:class="{'header-desktop mt-n12': $vuetify.breakpoint.mdAndUp, 'header-mobile mt-n6': $vuetify.breakpoint.xsOnly}")
                    span.redheader pleno centro&nbsp;
                    span de viña
                p.body Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            v-col().pr-0
                img(src="../assets/image.png" width="100%")
</template>

<script>
export default {
    data: () => ({
        windowHeight: window.innerHeight,
    })
}
</script>


<style>
    .margin-header-desktop {
        margin-left: 175px;
    }

    .my-subheader {
        font-size: 16px;
        color: #3eb3e5;
        font-family: "Roboto";
        margin-bottom: 10px;
    }

    .header-desktop {
        font-family: "Playfair Display";
        font-size: 80px;
        font-weight: 400;
        display: flex;
        color: #535b6c;
    }

    .header-mobile {
        font-family: "Playfair Display";
        font-size: 30px;
        font-weight: 400;
        display: flex;
        color: #535b6c;
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