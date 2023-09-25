<template>
   <ul>
    <li v-for="item in student" :key="item.id" class="list" >
  {{ item.name }}
    </li>
   </ul>

   <ul>
    <li v-for="item in student2" :key="item.id"  >
  {{ item }}
    </li>
   </ul>

    
</template>

<script>
export default{
    data(){
        return{
            message:"hello world!",
            info:"hii",
            student:[{name:"suraj",id:1},{name:"alex",id:2}],
            student2:["suraj","alex","bob"]

        }
    }
}


</script>

<style scoped>
.list{
    border:2px solid black;
    padding:10px;
    color:red;
    list-style: none;
    margin-bottom: 10px;
    font-size: 18px;

}

</style>