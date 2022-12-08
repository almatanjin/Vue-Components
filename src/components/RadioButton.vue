<template>
<h1>Get Checkbox & Radio button values</h1>
<div>
    <h3>Who am I?</h3>
</div>
<div>
    <label for="student">Student</label>
    <input type="radio" id="student" value="student" v-model="who" name="who"/>
</div>
<div>
    <label for="developer">Developer</label>
    <input type="radio" id="developer" value="developer" v-model="who" name="who" />
</div>
<h3>Language</h3>
<div>
<label for="java">Java</label>
<input id="java" type="checkbox" v-model="language" value="Java"/>
</div>
<div>
<label for="python">Python</label>
<input id="python" type="checkbox" v-model="language" value="python"/>
</div>

<div>
    <h4>I am {{who}}</h4>
</div>
<div>
    <h4>Selected Languauge {{language}}</h4>
</div>
</template>
<script>

export default{
    name:'RadioButton',

    data(){
        return {
            language:[],
            who:''
        }
    }
}


</script>
<style>


</style>