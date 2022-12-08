<template>
<h1>{{text}}</h1>
<div v-html="tag"></div>
<div :class="applyStyle">Home Component</div>
<div><Button v-on:click="(colorful=!colorful)">Color</Button></div>

</template>

<script>
export default{
  name:'HtmlText',

  data()
  {
    return {
        text:'alma',
        colorful:false,
        ht : 'blue',

        tag:'<h2>Hlw</h2>'
    }
  },
  methods:{
    myfunction(){
        this.colorful=!this.colorful
    },
    computed: {
        applyStyle() {
            return {
                green:this.colorful,
                blue:this.colorful
            }
        }
    }
  }

}

</script>

<style>

.pink{
    background-color: pink;
    width: 200px;
    display: flex;
    justify-content: center;


}
.blue{
    color: blue;
}
</style>