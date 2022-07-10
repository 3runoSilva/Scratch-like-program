<template>
  <HeaderComp />
  <router-view />
  <FooterComp />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HeaderComp from "./components/HeaderComp.vue";
import FooterComp from "./components/FooterComp.vue";

export default defineComponent({
  name: "app",
  components: {
    HeaderComp,
    FooterComp,
  },
});
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    text-decoration: none;
    color: #fdfeff;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
