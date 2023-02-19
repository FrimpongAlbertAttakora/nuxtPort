<template>
  <v-app :style="{background: $vuetify.theme.themes.dark.background}">
    <AppHeader/>
    <v-main>
      <nuxt />
    </v-main>
  </v-app>
</template>


<script>
import AppHeader from '../components/appHeader'
export default {
  components: {
    AppHeader
  }
}
</script>


<style>
*{
  background: midnightblue;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 1rem;
  line-height: 1.6;
}

a {
  color: #666;
  text-decoration: none;
}

ul {
  list-style: none;
}

.container {
  max-width: 800px;
  margin: 2rem auto;
  overflow: hidden;
  padding: 1rem 2rem;
  background: #fff;
}
</style>
