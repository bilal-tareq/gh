<template>
    <p> Hey {{ name }} and {{ numbere }} and mail{{ email }}</p>
  
    
    
</template>

<script setup>
import { defineProps } from 'vue';
const props = defineProps({

        name: String,
        numbere: Number,
        email: {type: String,}
        
});
</script>


<style scoped>
    p{
        color: blue;
    }
</style>