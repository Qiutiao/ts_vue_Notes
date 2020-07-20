<template>
  <div id="app">
    <MenuBar />
    <ItemList />
    <Editor v-if="$store.state.isShow" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import MenuBar from "./components/MenuBar.vue";
import ItemList from "./components/ItemList.vue";
import Editor from "./components/Editor.vue";

@Component({
  components: {
    MenuBar,
    ItemList,
    Editor
  }
})
export default class App extends Vue {}
</script>

<style>
</style>
