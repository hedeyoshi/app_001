<template>
  <div class="arms">
    <div class="arms-right"></div>
    <div class="arms-left"></div>
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
  right: 0;
  left: 0;
  .arms-right {
    position: absolute;
    top: 0;
    right: 24px;
    display: block;
    width: 72px;
    height: 200px;
    background-color: var(--color-body);
    border: 16px solid var(--color-line);
    border-top: none;
    border-radius: 0 0 36px 36px;
  }
  .arms-left {
    position: absolute;
    top: 0;
    left: 24px;
    display: block;
    width: 72px;
    height: 200px;
    background-color: var(--color-body);
    border: 16px solid var(--color-line);
    border-top: none;
    border-radius: 0 0 36px 36px;
  }
}
</style>
