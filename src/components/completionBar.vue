<template>
  <div>
    <h4>completion Bar</h4>
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

<style lang="css" scoped>
.wrapper {
  border-radius: 6px;
  height: 20px;
  width: 80vw;
  display: flex;
  justify-content: flex-start;
  background-color: #eee;
  overflow: hidden;
  box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.12);
}
.completion-block {
  background-color: blue;
  transition: width 1s cubic-bezier(0.165, 0.84, 0.44, 1);
}
</style>
