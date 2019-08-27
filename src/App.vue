<template lang="pug">
  v-app( style="background: white")
    nav-bar
    v-content
      Hero
      Services
      Ubication
</template>

<script>
import NavBar from './components/NavBar'
import Hero from './components/Hero'
import Services from './components/Services'
import Ubication from './components/Ubication'

export default {
  name: 'App',
  components: {
    NavBar, Hero, Services, Ubication
  }
};
</script>
