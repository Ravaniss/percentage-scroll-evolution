<template>
  <div id="app">
    <Post />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Post from './components/Post.vue'

@Component({
  components: {
    Post
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
  background-color: #F3F3F3;
}

#app {
  padding: 25px;
}
</style>
