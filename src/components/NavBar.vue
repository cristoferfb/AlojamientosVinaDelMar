<template lang="pug">
    div
        v-toolbar(flat :class="{'margin-desktop': $vuetify.breakpoint.lgAndUp}")
            v-toolbar-title.logo AVM
            div.line.d-none.d-sm-flex.ml-10.mr-5
            v-toolbar-items.d-none.d-sm-flex
                v-btn(text)
                    span.menuOption Servicios
                v-btn(text)
                    span.menuOption Ubicacion
                v-btn(text)
                    span.menuOption Contacto
            div.flex-grow-1
            v-toolbar-items.d-none.d-sm-flex
                v-btn(
                    text
                    href="https://www.facebook.com/Alojamientos-Viña-del-Mar-107616807270388"
                    target="_blank"
                )
                    v-img(
                        src="../assets/Facebook.png"
                        max-width="16"
                    )
                v-btn(text)
                    v-img(
                        src="../assets/Intagram.png"
                        max-width="16"
                    )
</template>

<style>
    .logo {
        font-family: 'Playfair Display', serif;
        font-weight: 700;
        color: #535b6c;
        font-size: 24px;
    }

    .line {
        width: 1px;
        height: 22px;
        border-left: solid #e7ebf2;
    }

    .menuOption {
        font-family: 'Roboto', sans-serif;
        font-size: 16px;
        color: #535b6c;
        font-weight: 400;
        text-transform: none;
    }

    .margin-desktop {
        margin-left: 159px;
        margin-right: 180px;
    }
</style>