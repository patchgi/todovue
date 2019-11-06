<template>
  <div class="home">
    <TodoForm></TodoForm>
    <TodoList></TodoList>
  </div>
</template>

<script lang="ts">
// @ is an alias to /src
import { Component, Vue } from "vue-property-decorator";
import TodoList from "@/components/TodoList.vue";
import TodoForm from "@/components/TodoForm.vue";

@Component({
  components: {
    TodoList,
    TodoForm
  }
})
export default class Home extends Vue {}
</script>
