<template>
    <h1>Alma</h1>
    <input id="input" type="text" v-model="count"/>
    <h1>{{count}}</h1>
    <button v-on:click="countValue()">Click</button>
</template>
<script>
export default{
    name: 'HomePro',
    data(){
        return {
            count:''
        }
    },
    methods:{
     countValue(){

        alert( this.count.length)

     }
    }
}
</script>