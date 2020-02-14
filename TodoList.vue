<template>
  <div v-bind:class="{ active: counter > 3, container: true }">Hello {{name}}
    <button v-on:click="counter += 1">Add 1</button>
  <p>Se ha hecho clic en el botón de arriba {{ counter }} veces.</p>
  </div>
</template>

<script lang="ts">
import Vue from "vue";


export default Vue.extend({
  data: () => ({
      name: "Jairo",
      counter: 0
  })
});
</script>

<style lang="scss" scoped>
.container {
  color:blue;
  border:1px solid gray;
  width: 500px;
  padding: 10px;
}

.active {
  background-color: red;
}
</style>