<template>
   <div class="container">
    <div class="box">
        <div class="box1"></div>
        <div class="box1"></div>
    </div>
    <div class="box">
        <div class="box2"></div>
        <div class="box2"></div>
    </div>
   </div>
   
</template>
<style scoped>

.container{
    border:1px solid black;

}

.box{
    display:flex;
    justify-content: space-between;
}

.box1{
    border:1px solid black;
    background:blue;
    width:100px;
    height:100px;
}

.box2{
    border:1px solid black;
    background:blue;
}
</style>

