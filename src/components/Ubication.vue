<template lang="pug">
    v-container(id="ubication")
        v-container.text-center
            p(:class="{'services-header-mobile': $vuetify.breakpoint.mdAndDown}").services-header.mb-0.pb-0 Ubicación
            p.body Nos encontramos en Av. Agua Santa N°22, Viña del Mar, una ubicacion privilegiada por su cercania a varios puntos de interes de la ciudad como rapido acceso a distintos medios de locomocion con lo que se dispone de diferentes opciones para llegar a practicamente cualquier lugar de Viña y Valparaiso. 
        v-row(align="center").text-center
            v-col(cols="12")
                v-card(flat)
                    iframe(
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3345.1913577141263!2d-71.56510148420446!3d-33.02508868319462!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9689ddfd7034bfd7%3A0xcd3290503bfa4012!2sAgua%20Santa%2022%2C%20Vi%C3%B1a%20del%20Mar%2C%20Regi%C3%B3n%20de%20Valpara%C3%ADso!5e0!3m2!1ses-419!2scl!4v1566863952874!5m2!1ses-419!2scl"
                        width="600"
                        height="450"
                        frameborder="0"
                        :class="{'responsive-map': $vuetify.breakpoint.mdAndDown}"
                    )
            v-col(cols="12").d-flex.d-md-none
                v-row
                    v-col
                        v-btn(:href="gmapslink" color="success" :block="$vuetify.breakpoint.smAndDown").pa-10
                            v-icon(left) mdi-map
                            span Abrir en Google maps
                    v-col
                        v-btn(:href="uberlink" color="black" dark :block="$vuetify.breakpoint.smAndDown").pa-10
                            v-icon(left) mdi-taxi
                            span Viajar en Uber
</template>

<script>
export default {
    data: () => {
        return {
            gmapslink: "http://maps.google.com/?q=Agua+Santa+22,+Viña+del+Mar,+Región+de+Valparaíso",
            uberlink: "https://m.uber.com/ul/?action=setPickup&client_id=5LdeY80FokDdUJcAWKNWlSDvSRozhOhS&pickup=my_location&dropoff[formatted_address]=Agua%20Santa%2022%2C%20Vi%C3%B1a%20del%20Mar%2C%20Chile&dropoff[latitude]=-33.025093&dropoff[longitude]=-71.562913"
        }
    }
}
</script>

<style>
    .responsive-map {
        width: 100%;
    }
</style>