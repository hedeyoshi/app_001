<template>
  <div class="arms">
    <div class="arms-right">みぎうで</div>
    <div class="arms-left">ひだりうで</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.arms {
  position: absolute;
  top: 40%;
  .arms-right {
    background-color: #fff;
  }
  .arms-left {
    background-color: #fff;
  }
}
</style>
