<template>
    <p v-bind:style="{
    backgroundColor: '#ccc', color: color}" >El mensaje se ha enviado satisfactoriamente</p>
    <button v-on:click="handclick">Cambiar color</button>

</template>

<script setup>
    import { ref } from "vue";
        let color =ref('#fff')
        const handclick = () => {color.value = '#ff0000'}
</script>

<style scoped>

</style>