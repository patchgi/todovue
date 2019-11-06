<template>
  <form class="add-form" @submit.prevent="add">
    <input type="text" ref="comment" />
    <button type="submit">追加</button>
  </form>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({})
export default class TodoForm extends Vue {
  public add() {
    var $comment: Object;
    $comment = this.$refs.comment;
  }
}
</script>