<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <study></study> -->
    <!-- <App2/> -->
    <!-- <test1></test1> -->
    <MyComponent />
    <Test2 />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import App2 from './App2.vue'
// import study from './components/study.vue'
// import test1 from './components/test1.vue'
import MyComponent from './components/MyComponent.vue'
import Test2 from './components/Test2.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    //study,
    //test1,
    MyComponent,
    Test2
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
