<template>

    <HelloWorld msg="Welcome Alma"/>
     <HomePro/>
     <MessageVue msg="Hi" />
     <CountVue msg="I am  from count" />
     <ShowInfo />
    </template>
    
    <script>
    import CountVue from './components/CountVue.vue';
    import HelloWorld from './components/HelloWorld.vue'
    import HomePro from './components/HomePro.vue';
    import MessageVue from './components/MessageVue.vue';
    import ShowInfo from './components/ShowInfo.vue';
    
    
    export default {
      name: 'App',
      components: {
        HelloWorld,
        HomePro,
        MessageVue,
        CountVue,
        ShowInfo
    }
    }
    </script>
    
    <style>
    #app {
      font-family: Avenir, Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-align: center;
      color: #2c3e50;
      margin-top: 60px;
    }
    </style>









    <template>

      <h1>Welcome</h1>
      <RadioButton />
      </template>
      
      <script>
      import RadioButton from './components/RadioButton.vue';
      
      
      
      
      export default{
          components: { RadioButton }
      }
      
      
      </script>
      <style>
          #app {
            font-family: Avenir, Helvetica, Arial, sans-serif;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
            text-align: center;
            color: #2c3e50;
            margin-top: 60px;
          }
          </style>






          