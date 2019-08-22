<template lang="pug">
  v-app( style="background: white")
    nav-bar
    v-content
      div
</template>

<script>
import NavBar from './components/NavBar'

export default {
  name: 'App',
  components: {
    NavBar
  }
};
</script>
