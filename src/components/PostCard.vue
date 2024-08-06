<template>
    <div class="post-card">
        <!-- post card con texto y el componente postbtn insertado -->
        <h3>Título</h3> 
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo corrupti nihil consectetur cum vel a 
            iusto quam, beatae ducimus eaque praesentium, deserunt nesciunt cupiditate, reiciendis voluptates sed. 
            Maxime, dolor laboriosam.
        </p>
        <PostBtn/>
    </div>
</template>

<script setup>
    import PostBtn from './PostBtn.vue';
</script>

<style scoped>
.post-card {
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>