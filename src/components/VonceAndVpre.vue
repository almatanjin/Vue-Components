<template>
<h2>Do you like Tacos?</h2>
<textarea v-model="show" @keyup.enter="addComment" ></textarea>
<pre>{{show}}</pre>
<ul>
    <li v-for="item in comments" :key="item" ref="in">{{item}}</li>
</ul>
<input type="text" v-model="newcomments" @keyup.enter="addComment" />
<br />
<div>


    <input type="text" ref="input" />
    <button @click="myfunction()">Click</button>
    <p>{{val}}</p>
</div>

</template>

<script>



export default{
    name:'VonceAndVpre',
    data(){
        return{
            show:"I love Tacos",
            newcomments:'',
            val:'',
            comments:[
                
                
            ]
        }
    },
    methods:{

        addComment(){
            this.$refs.in.value.style.color="red"
            this.comments.push(this.newcomments)
            this.newcomments=""
            
            
        },
        myfunction (){
            this.$refs.input.style.color="blue";
            this.$refs.input.focus();
            this.val = this.$refs.input.value;




        }

        

    }
}



</script>

<style>


</style>