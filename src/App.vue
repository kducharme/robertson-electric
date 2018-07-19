<template>
  <div class="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
* {
  margin: 0;
  box-sizing: border-box;
  font-family: "Lato", "Merriweather";
}
.app {
  margin: 0 0 32px 0;
}
</style>
