<template>
  <div id="app">
    <AboutMe></AboutMe>
    <CompletionBar/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import CompletionBar from "./components/completionBar";
import AboutMe from "./components/AboutMe";

export default {
  name: "App",
  components: {
    HelloWorld,
    CompletionBar,
    AboutMe
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
