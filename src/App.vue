<template lang="pug">
  v-app( style="background: white")
    nav-bar
    v-content
      Hero
      Services
</template>

<script>
import NavBar from './components/NavBar'
import Hero from './components/Hero'
import Services from './components/Services'

export default {
  name: 'App',
  components: {
    NavBar, Hero, Services
  }
};
</script>
