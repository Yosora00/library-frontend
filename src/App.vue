<template>
  <div id="app">
    <nav-bar></nav-bar>
    <router-view class="container" style="margin-top: 25px"></router-view>
  </div>
</template>

<script>
import NavBar from "components/common/NavBar";
export default {
  name: "App",
  components: { NavBar },
};
</script>
<style>
</style>
