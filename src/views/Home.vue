<template>
  <div class="home">
    <HelloWorld />
    <Snake />
  </div>
</template>

<script>
// @ is an alias to /src
import Snake from "@/components/Snake.vue";
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "home",
  components: {
    Snake,
    HelloWorld
  }
};
</script>
