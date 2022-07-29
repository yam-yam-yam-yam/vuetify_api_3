<template>
  <v-app id="main">
    <v-tabs
      v-model="tab"
      align-with-title
    >
      <v-tab
        v-for="item in items"
        :key="item"
        :value="item"
      >
      {{item}}
      </v-tab>
    </v-tabs>
    <v-window>
      <component :is="tab"></component>
    </v-window>
  </v-app>

</template>

<script>
import AlertComponent from './components/Alert.vue'
import AppBarComponent from './components/AppBar.vue'
import AvatarsComponent from './components/Avatars.vue'

export default {
  name: 'AppComponent',
  components: {
    AlertComponent,
    AppBarComponent,
    AvatarsComponent
  },
  data() {
    return {
      tab:undefined,
      items:[
        'AlertComponent',
        'AppBarComponent',
        'AvatarsComponent'
      ]
    }
  },
}
</script>

<style>
#main > * {
  padding:3%;
}
</style>