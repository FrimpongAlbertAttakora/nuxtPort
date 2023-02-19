<template>
    <div id="app">
      <typewriter
        :replace="replace"
        :type-interval="100"
        :replace-interval="1000"
      >
        <div style="font-size: 30px; color: gray; text-decoration: underline"> Hello, I am a full stack developer </div>
      </typewriter>
    </div>
  </template>


<script>
import Typewriter from "typewriter-vue";

export default {
  name: "App",
  components: {
    Typewriter,
  },
  data: () => ({
    replace: [
      { from: "full stack developer", to: "mathematics educator" },
      { from: "Hello, I am a mathematics educator", to: " ... and an electronics hobbist base in Ghana" },
      { from: " ... and an electronics hobbist base in Ghana" , to: " Hello, I am a full stack developer ... base in Ghana" },
    ],
  }),
};
</script>

<style>
.typewriter.content *:last-child::after {
  font-size: calc(3em + 20px) !important;
}
</style>