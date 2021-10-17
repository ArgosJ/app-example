<template>
  <div id="app">
    <HelloWorld msg="Hello World" />
    <Example :items="items" />
  </div>
</template>

<script>
import Example from "./components/Example.vue";
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Example
  },
  data() {
    return {
      items: [
        {
          name: "Owen",
          lastName: "Yaipen"
        },
        {
          name: "Jackson",
          lastName: "Yaipen"
        }
      ]
    };
  }
};
</script>

<style lang="scss">
@import "~@/assets/scss/vendors/bootstrap-vue/index";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
