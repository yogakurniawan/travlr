<template>
  <div class="hello">
    <navbar></navbar>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar/index.vue";

export default {
  components: {
    Navbar
  },
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
