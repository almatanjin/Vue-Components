<template>
    <img v-if="seek" src="https://gifdb.com/images/high/panda-dance-pixel-cartoon-z84rac6645a9xl22.gif" height="150" />
    <div><button v-on:click="myfunction()">Hide and Seek</button></div>
    <div>
        <h1>For loop in Vue js</h1>
    </div>
    <ul>
        <li v-for="item in language" :key="item">
            {{item}}

        </li>
    </ul>
    <br />
    <br />
    <ul>
        <li v-for="item in user" :key="item.name">

            Name : {{item.name}} <br /> Email : {{item.email}}
        </li>
    </ul>
</template>
<script>
export default{
    name:"HideSeek",
    data(){
        return {
            seek:false,
            language:['java','node','php','html'],
            user:[
                {
                    name:"Alma",
                    email:"alma@softzino.com"
                },
                {
                    name:"Tanjin",
                    email:"alma@softzino.com"
                },
                {
                    name:"Tania",
                    email:"alma@softzino.com"
                }
            ]
        }
    },

    methods:{
        myfunction(){
            this.seek=!this.seek;
        }

    }

}
</script>
<style>

</style>