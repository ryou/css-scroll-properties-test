<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline">
        <span>CSS Scroll Properties</span>
      </v-toolbar-title>
    </v-toolbar>

    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data() {
    return {
      //
    };
  },
};
</script>

<style lang="scss">
html {
  overscroll-behavior: none;
}
</style>

