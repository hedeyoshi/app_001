<template>
  <div class="head">
    <div class="ears">
      <div class="ears-right"></div>
      <div class="ears-left"></div>
    </div>
    <div class="eyes">
      <div class="eyes-right"></div>
      <div class="eyes-left"></div>
    </div>
    <div class="mouth"></div>
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
    position: absolute;
    top: -64px;
    left: 0;
    right: 0;
    &-right {
      position: absolute;
      top: 0;
      right: 40px;
      width: 0;
      height: 0;
      border-right: 32px solid transparent;
      border-left: 32px solid transparent;
      border-bottom: 64px solid var(--color-line);
      &::after {
        content: '';
        position: absolute;
        display: block;
        top: 28px;
        right: -24px;
        border-right: 24px solid transparent;
        border-left: 24px solid transparent;
        border-bottom: 48px solid var(--color-body);
      }
    }
    &-left {
      position: absolute;
      top: 0;
      left: 40px;
      width: 0;
      height: 0;
      border-right: 32px solid transparent;
      border-left: 32px solid transparent;
      border-bottom: 64px solid var(--color-line);
      &::after {
        content: '';
        position: absolute;
        display: block;
        top: 28px;
        left: -24px;
        border-right: 24px solid transparent;
        border-left: 24px solid transparent;
        border-bottom: 48px solid var(--color-body);
      }
    }
  }
  .eyes {
    position: absolute;
    top: 20px;
    left: 0;
    right: 0;
    background: #ccc;
    &-right {
      content: '';
      position: absolute;
      top: 0;
      right: 82px;
      width: 16px;
      height: 16px;
      border-radius: 12px;
      background-color: var(--color-line);
    }
    &-left {
      content: '';
      position: absolute;
      top: 0;
      left: 82px;
      width: 16px;
      height: 16px;
      border-radius: 12px;
      background-color: var(--color-line);
    }
  }
  .mouth {
    position: absolute;
    top: 48px;
    left: 92px;
    right: 92px;
    height: 16px;
    background-color: var(--color-bg);
    border-radius: 8px;
    // border-right: 10vw solid transparent;
    // border-left: 10vw solid transparent;
    // border-top: 4vw solid var(--color-bg);
  }
}
</style>
