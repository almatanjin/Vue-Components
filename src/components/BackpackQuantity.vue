<template>
    <div class="con">

<img src="https://static.vecteezy.com/system/resources/previews/009/384/957/original/backpack-set-clipart-design-illustration-free-png.png" width="235" height="300"/>
<div class="container">
    <div><button @click="(counter >0)? counter-=1 : 0">-</button></div>
<div> Quantity : {{counter}}</div>
<div> <button @click=" counter+=1 ">+</button></div>

</div>
</div>
</template>

<script>
export default{
    name:"BackpackQuantity",
    data(){
        return{
            counter:0
        }
    }
}


</script>

<style>
.container{
    display: flex;
    gap: 20px;
    
}

.con{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 20px;
}


</style>