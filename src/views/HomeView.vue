<template>
  <div class="home"><h1></h1></div>
  <router-view> </router-view>
  <HelloWorld></HelloWorld>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
  },
};
</script>
