<template>

    
<VonceAndVpre />
<ParentVue />
<ChildVue />



</template>

<script>





import ChildVue from './components/ChildVue.vue';
import ParentVue from './components/ParentVue.vue';
import VonceAndVpre from './components/VonceAndVpre.vue';





export default{
    components: { VonceAndVpre, ParentVue,  ChildVue }
}


</script>

<style>


</style>