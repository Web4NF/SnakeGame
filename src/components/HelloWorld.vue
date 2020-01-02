<template>
  <div class="hello">
    <!-- <div
      class="test"
      @touchstart="gtouchstart()"
      @touchmove="gtouchmove()"
      @touchend="gtouchend()"
    >touchDemo</div>-->

    <v-touch
      @swipeleft="swipeleft"
      @swiperight="swiperight"
      @swipeup="swipeup"
      @swipedown="swipedown"
    >
      <div class="test">v-touch Demo</div>
    </v-touch>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    // gtouchstart() {
    //   console.log("1，按下");
    // },
    // gtouchmove() {
    //   console.log("2，按下移动");
    // },
    // gtouchend() {
    //   console.log("3，松开");
    // },
    swipeleft() {
      console.log("左划");
    },
    swiperight() {
      console.log("右滑");
    },
    swipedown() {
      console.log("下滑");
    },
    swipeup() {
      console.log("上滑");
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.test {
  width: 100%;
  height: 50px;
  text-align: center;
  background-color: red;
  line-height: 50px;
  font-size: 20px;
}
</style>
