<template >
  <div>
    <p>Hello {{name}}</p>
    <TodoList />
  </div>
</template>

<script>
import TodoList from "./TodoList.vue";

export default {
  components: {
    TodoList
  },
  data() {
    return {
      name: "Olga"
    };
  }
};
</script>

<style lang="scss" scoped>
div{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
p {
  color: green;
}
</style>