<template>
    <div class="container">

    <h1>Name: {{getName('Alma')}} </h1>
    <h1>Email: {{getEmail('alma@softzino.com')}}</h1>
    <h1>Mobile: {{getMobile('01990-747505')}}</h1>
    <h1> Info: {{getData()}}</h1>
    
    <h1> {{count}}</h1>
    
    
</div>
<div><button v-on:dblclick="doubble('I am click')">Click </button></div>
<button v-on:click="test()">Click </button>
<div>
    <button v-on:click="myfunction()"> count</button>
</div>

</template>
<script>

export default{
name: 'ShowInfo',

data(){
    return {
        location:"Uttara",
        count:0,
       getEmail:function(a)
       {
        return a;
       },
       getName:function(a){
        return a;
       },
       getMobile:function(a){
        return a;
       }

    }
},

methods:{
    getData(){
        return {
            name: 'alma',
            email: 'tanjin@softzino.com'
        }

    },
    getLocation(){
        
        return this.location;
    },
    test(){
        alert(this.getLocation());
    },
    doubble(input){
        alert(input)
    },
    myfunction(){
        this.count++;
       
    }
}


    

}

</script>
<style scoped >


h1{
    font-size: medium;
}
.container{
    display: flex;
    flex-direction: column;
    color: palevioletred;
    
    margin: auto;
    border: 2px solid black;
    width: 300px;
    text-align: left;
    padding-left: 4px;
}

</style>