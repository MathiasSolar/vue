<template>
    <div class="post-card">
        <h3>Titulo</h3>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tenetur, possimus magnam et repudiandae dolorum laboriosam molestiae dolor expedita libero dolores suscipit qui, quis aspernatur illo doloribus error impedit dolore delectus. </p>   
        <PostButton/>
    </div>
</template>

<script setup>
    import PostButton from './PostButton.vue';
</script>

<style scoped>
.post-card{
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>