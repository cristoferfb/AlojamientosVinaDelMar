<template lang="pug">
  v-app( style="background: white")
    nav-bar
    v-content
      Hero
      Services
      Ubication
      Contact
      Footer
</template>

<script>
import NavBar from './components/NavBar'
import Hero from './components/Hero'
import Services from './components/Services'
import Ubication from './components/Ubication'
import Contact from './components/Contact'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    NavBar, Hero, Services, Ubication, Contact, Footer
  }
};
</script>
