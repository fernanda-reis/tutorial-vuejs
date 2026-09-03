<template>
  <header>
    <h1 :style="{ color: titleColor }">{{ title }}</h1>
    <button @click="handleClick()" :style="{ backgroundColor: bgColor }">
      {{ action }}
    </button>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    title: String,
    action: String,
    titleColor: String,
    bgColor: String,
  },

  methods: {
    handleClick() {
      console.log("hey, you clicked me");
    },
  },
};
</script>

<style>
button {
  padding: 10px 20px;
  background-color: seagreen;
  font-size: 16px;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

h1 {
  color: greenyellow;
}
</style>
