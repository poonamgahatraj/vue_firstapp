<template>
  <h1>Hello</h1>
  <h2 @click="change">poonam</h2>
  <h2 v-if="show_message" >Hello I will visible</h2>
</template>
<script setup>
import { ref } from 'vue'
const show_message=ref(true);

function change()
{
    console.log(show_message)
    show_message.value=!show_message.value;
}
</script>
