<template>
<h1>Parent component</h1>
<ChildVueVue name="Alma Tanjin" :user="user" :getData="getData" :getname="getName" />

</template>
<script>


import ChildVueVue from './ChildVue.vue';
export default{

    name:'ParentVue',
    components:{
        ChildVueVue

    },
    data()
    {
        return {
            user:{name:'Shaan',email:'shaan@gmail.com'}
        }

    },
    methods:{
        getData(){
            alert('hi');
        },
        getName(){
            alert('Alma');
        }
    }
}

</script>
<style>

</style>