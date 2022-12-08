<template>
<h1>What is your favorite kind of Taco ?</h1>
<textarea v-model="show" v-if="none"></textarea>

<div><button id='button' v-if="show" type="submit" v-on:click="myfunction()">Let us know?</button></div>
<div>{{value}}</div>


<div>
    <h1>Do you like Taco?</h1>
    <div>
        <label for="yes">Yes</label>
        <input type="radio" value="yes" name="who" v-model="option"/>
    </div>
    <div>
        <label for="no">No</label>
        <input type="radio" value="no" name="who" v-model="option"/>
    </div>
    <h3 v-if="(option==='yes')">Yes</h3>
    <h3 v-else-if="(option==='no')"> Uhu</h3>
</div>

</template>

<script>
export default{
    name:'TacosV',
    
    data(){
        return {
            show:"",
            none: true,
            value:"",
            option:"",
        }
    },

    methods:{
        myfunction(){
            this.none=false
            this.value=this.show
            this.show=""


        }
    }
}


</script>

<style>
#button{
    background-color: orange;
    border:none;
    padding: 10px;
    color: aliceblue;
}

</style>