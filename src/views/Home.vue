<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Example :items="sons"/>
    <Example :items="parents"/>
  </div>
</template>

<script>
import Example from '@/components/Example.vue'
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld, Example
  },
  data() {
    return {
      sons: [
        {
          name: "Aldair",
          lastName: "Yaipen"
        },
        {
          name: "Emely",
          lastName: "Yaipen"
        }
      ],
      parents: [
        {
          name: "Victor",
          lastName: "Yaipen"
        },
        {
          name: "Yolanda",
          lastName: "Saba"
        }
      ]

    };
  }
}

</script>
