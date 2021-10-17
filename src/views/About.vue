<template>
  <div class="about">
    <Example :items="items" />
  </div>
</template>
<script>
import Example from '@/components/Example.vue'
export default ({
  name: 'About',
  components: {
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
})
</script>
