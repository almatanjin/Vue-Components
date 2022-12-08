<template>
<h2>{{name}}</h2>
<h2>{{user.nam0}}</h2>
<button v-on:click="getData()">Call Function</button>
<button @click="getname()">Get Name</button>
</template>
<script>


export default{
    name:'ChildVue',
    props:{
        name:String,
        user:Object,
        getData:Function,
        getname:Function
       
    }
    
}
</script>
<style>

</style>