<template>
  <div class="container">
    <Header
      title="* Vue App *"
      action="Click me"
      titleColor="purple"
      bgColor="#8f0303"
    />
  </div>
  <div class="container">
    <Header title="* Vue App 2*" action="Click me too" />
  </div>
</template>

<script>
import Header from "./Header.vue";
export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style>
#app {
  text-align: center;
  color: yellowgreen;
  margin: 60px;
}

.container {
  border: 1px solid steelblue;
  padding: 30px;
  max-width: 500px;
  margin: 20px auto;
}
</style>
