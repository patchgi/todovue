<template>
  <tbody>
    <tr v-for="item in todos" v-bind:key="item.id">
      <td>{{ item.id }}</td>
      <td>{{ item.comment }}</td>
      <td class="state">
        <!-- 状態変更ボタンのモック -->
        <button>{{ item.state }}</button>
      </td>
      <td class="button">
        <!-- 削除ボタンのモック -->
        <button>削除</button>
      </td>
    </tr>
  </tbody>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component({})
export default class TodoList extends Vue {}
</script>