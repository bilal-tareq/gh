<template>
    <p> You clicked me {{ count }} times.</p> 
    <button @click="count++">You clicked me  + .</button>
    <button @click="count--">You clicked me -.</button>
   
    <p> {{ count > 0 ? "pos":"neg" }}</p>
    <slot></slot>
 </template>


<script setup> 
    import { ref } from 'vue';
    const count = ref(0);
    
</script>



<style scoped>
    p{
        color: red;
    }

</style>