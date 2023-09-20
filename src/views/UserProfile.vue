<script setup>
import {ref} from 'vue'
 import {useRoute} from 'vue-router'

const route = useRoute()
const  profile = ref('Hi, This is Mr.'+ route.params.username)
</script>

<template>
  <main>
   <h1>{{profile}}  </h1>
   <p>Nice to meet you.</p>
  </main>
</template>

<style scoped >
main{
    background: #ddd;
    border: 10px solid #41b883;
    text-align: center;
}
</style>