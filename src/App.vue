<template>
  <div class="">
    <img alt="Vue logo" src="./assets/logo.png" />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- <Home propname="hello this is prop" /> -->
    <!-- <Home proptwo="this is second prop" /> -->
    <!-- <Fordirective /> -->
    <!-- <Signup /> -->
    <SignUpTwo />
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
// import Home from "./components/Home.vue";
// import Fordirective from "./components/Fordirective.vue";
// import Signup from "./components/Signup.vue";

import SignUpTwo from "./components/SignUpTwo.vue";
export default {
  name: "App",
  components: {
    // HelloWorld,
    // Home,
    // Fordirective,
    // Signup,
    SignUpTwo,
  },
};
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
