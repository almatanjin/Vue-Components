<template>
<div>
    <p v-for="(item, key , index) in jokes" :key="item">{{index}} . {{key}} : {{item}} </p>
</div>

</template>

<script>
import { createForLoopParams } from '@vue/compiler-core';

export default{
    name:createForLoopParams,
    data(){
        return{
            jokes:{
                qus:'What did one baby prototype say to the other?',
                ans:"I'll race you to class!",
                response:"groan"
            }
        }
    }
}

</script>


<style>


</style>