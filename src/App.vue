<template>
  <h1>Listado de posts</h1>
  <post-container/>
</template>

<script lang="ts">
import { defineComponent, DefineComponent } from 'vue';
import PostContainer from './components/PostContainer.vue';
export default defineComponent({
  components: {
    PostContainer
  }
})
</script>

<style lang="scss">

</style>
