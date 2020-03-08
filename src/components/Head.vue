<template>
  <div class="head">
    <div class="ears">
      <div class="ears-right"></div>
      <div class="ears-left"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Head',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.head {
  .ears {
    &-right {
      width: 0;
      height: 0;
      border-right: 30px solid transparent;
      border-left: 30px solid transparent;
      border-bottom: 30px solid #000;
    }
  }
}
</style>
