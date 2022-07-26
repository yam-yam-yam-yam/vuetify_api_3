<template>
  <v-app id="main">
    <AlertComponent></AlertComponent>
  </v-app>
</template>

<script>
import AlertComponent from './components/Alert.vue'

export default {
  name: 'AppComponent',
  components: {
    AlertComponent
  }
}
</script>

<style>
#main > * {
  padding:3%;
}
</style>