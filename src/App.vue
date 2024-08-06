<template>
  <div>
    <h3>Listado de post</h3>
    <!-- post container tiene dentro de si a post card y post card tiene postbtn para entender el posicionamiento en cada elemento -->
    <!-- se agrega contador para ver comportamiento -->
    <CounterOption />
    <PostContainer />   
    <CounterComposition />
  </div>
</template>

<script setup>
  import PostContainer from './components/PostContainer.vue';
   import CounterOption from './components/CounterOption.vue';
  import CounterComposition from './components/CounterComposition.vue';
</script>

<style scoped>
h3 {
  color: purple;
}
</style>
