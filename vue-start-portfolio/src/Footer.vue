<template>
  <div :class="['footer', className]"></div>
</template>

<script>
export default {
  name: "Footer",
  props: {
    className: {
      type: String,
      default: ""
    }
  }
};
</script>

<style>
.footer {
  height: 80px;
  position: relative;
  width: 100%;
  max-width: 1420px;
  margin: 0 auto;
}
</style>