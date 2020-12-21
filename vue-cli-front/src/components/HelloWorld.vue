<template>
  <div @click="$emit('click-fn')" class="bg-blue-100">
    <h1>Hello {{ name }} 😁</h1>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    name: String,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bg-blue-100 {
  background-color: aqua;
}
</style>
