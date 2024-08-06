<template>
    <div class="post-container">
        <!-- container sirve como cajonera para almacenar a postcard -->
        <PostCard />
        <PostCard />
        <PostCard />
        <PostCard />
    </div>
</template>

<script setup>
import PostCard from './PostCard.vue';
</script>

<style scoped>
.post-container {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
}
</style>