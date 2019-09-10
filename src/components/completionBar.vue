<template>
  <div>
    <div class="wrapper">
      <div :style="{width:p+'%'}" class="completion-block"></div>
    </div>
  </div>
</template>

<script lang="js">
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      p: 0
    };
  },
  mounted() {
  let a = ()=>{
    setTimeout(() => {
      this.p = (this.p+20)%100;
      a();
    }, 2000);
  } 
  a();
  }
});
</script>

<style lang="scss" scoped>
.wrapper {
  border-radius: 6px;
  height: 20px;
  width: 80vw;
  display: flex;
  justify-content: flex-start;
  background-color: brown;
  overflow: hidden;
}
.completion-block {
  background-color: aqua;
  transition: width 1s cubic-bezier(0.165, 0.84, 0.44, 1);
}
</style>
