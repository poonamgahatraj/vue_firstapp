<template>
    <h1>my first page</h1>
    <div style="display:flex">
        <div>
            <box/>
            <box style="background:red"/>
        </div>
       <div>
        <box/>
        <box/>
       </div>
   
    </div>
    
</template>
<script setup>
import box from '../components/box.vue';
</script>