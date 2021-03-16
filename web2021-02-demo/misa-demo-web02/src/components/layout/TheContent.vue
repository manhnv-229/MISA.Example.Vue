<template>
  <div>
    <div id="content">
       <router-view></router-view>
    </div>
  </div>
</template>

<script>
// import CustomerList from "../../components/page/dictionary/customer/CustomerList.vue";

export default {
  name: "App",
  components: {
    // CustomerList
  },
};
</script>
<style scoped>
#content {
  position: absolute;
  top: 60px;
  left: 200px;
  right: 0px;
  bottom: 0px;
  /* background-color: yellow; */
  /* padding-left:  24px; */
  padding: 24px;
}
</style>