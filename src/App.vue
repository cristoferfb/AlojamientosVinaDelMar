<template lang="pug">
  v-app( style="background: white")
    nav-bar
    v-content
      Hero
</template>

<script>
import NavBar from './components/NavBar'
import Hero from './components/Hero'

export default {
  name: 'App',
  components: {
    NavBar, Hero
  }
};
</script>
