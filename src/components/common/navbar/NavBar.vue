<template>
  <div class="nav_bar">
    <div class="left">
      <slot name="left"></slot>
    </div>
    <div class="center">
      <slot name="center"></slot>
    </div>
    <div class="right">
      <slot name="right"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style scoped>
.nav_bar {
  display: flex;
  height: 44px;
  line-height: 44px;
}
.nav_bar .center {
  flex: 1;
}
.nav_bar .left,.nav_bar .right {
  width: 60px;
}

</style>