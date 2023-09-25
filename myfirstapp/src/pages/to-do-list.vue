<template>
    <div>

    
    <div style="display:flex;justify-content: flex-end;">
        <h2 >Hello {{ username.name }} your last login date is {{ username.date }}</h2>
    </div>
       
   
   
    <div class="container" >
       
        <div class="content2">
           <div v-for="item in task" class="item">
            <h3 style="display:flex; justify-content: center;"> {{ item.title }}</h3>
            <p style="display:flex; justify-content: center;">{{ item.description }}</p>
           
           </div>
          
        
        </div>
    </div>
    <button @click="HelloWorld">Click me</button>
    <input v-if="showaddform" type="text">
</div>
</template>

<style scoped>




.content2{
    border:2px solid black;
    height:400px;
   
    background:paleturquoise;
}

.item{
    border:1px solid black;
    
    background:burlywood;
    border-radius:50px;
    border:none;
    margin-top:10px;
    
}
</style>

<script>
import HelloWorld from '../components/HelloWorld.vue';


export default{
    data(){
        return{
            task:[{title:"hello",description:"lksl"},{title:"jfkjh",description:"jcolvflo"},{title:"klksdj",description:"jckjkcldv"}],
            username:{name:"suraj",date:"20th of december"},
           
            showaddform:false
        }
    },
    methods:
    {
        HelloWorld()
        {
           this.showaddform=!this.showaddform


        }
       
    }
}
 
</script>