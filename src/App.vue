<template>
  <div id="app">
    <Header />
    <router-view></router-view>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Header from "./layouts/Header/Header.vue";

@Component({
  components: {
    Header
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
@import "./assets/styles/variables.scss";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #333333;
}
</style>
