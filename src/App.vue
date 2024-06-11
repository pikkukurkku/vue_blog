<template>
  <div class="home">
    home
    <p>My name is {{ name }} and my age is {{ age }}</p>
    <button @click="handleClick">click me</button>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  name: "Home",
  setup() {
    console.log(this)

    const p = ref

    let name = "mario";
    let age = 30;

    const handleClick = () => {
      console.log("you clicked me");
    };

    return { name, age, handleClick };
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
}
</style>
