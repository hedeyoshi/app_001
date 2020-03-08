<template>
  <div class="legs">
    <div class="legs-right"></div>
    <div class="legs-left"></div>
  </div>
</template>

<script>
export default {
  name: 'Legs',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.legs {
  position: absolute;
  right: 0;
  left: 0;
  bottom: 0;
  background-color: #fff;
  .legs-right {
    position: absolute;
    top: 0;
    right: 24px;
    display: block;
    width: 72px;
    height: 20000px;
    background-color: var(--color-body);
    border: 16px solid var(--color-line);
    border-radius: 0 0 36px 36px;
  }
  .legs-left {
    position: absolute;
    top: 0;
    left: 24px;
    display: block;
    width: 72px;
    height: 20000px;
    background-color: var(--color-body);
    border: 16px solid var(--color-line);
    border-radius: 0 0 36px 36px;
  }
}
</style>
