<template>
  <div id="app">
    <TheMenu />
    <TheHeader />
    <TheContent />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TheHeader from "./components/layout/TheHeader.vue";
import TheMenu from "./components/layout/TheMenu.vue";
import TheContent from "./components/layout/TheContent.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    TheMenu,
    TheContent,
  },
};
</script>


<style>
@import "./css/main.css";
@import "./css/components/button.css";
@import "./css/components/text-box.css";
@import "./css/components/table.css";
@import "./css/components/dialog.css";
</style>
