<template>

<h1 class="vue">{{msg}}</h1>

</template>

<script>

export default{
    name:'CountVue',
    props:{
        msg:String
    }
}

</script>
<style scoped>

h1{
    color: orange;
}
</style>