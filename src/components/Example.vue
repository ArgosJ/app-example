<template>
  <div>
    Example component
    <ul class="list-group">
      <li class="list-group-item active" v-for="(item, index) in items" :key="index">
         <strong>{{ item.name }}</strong> ({{item.lastName}} apellido) 
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Example",
  props: {
    items: Array
  }
};
</script>

<style></style>
