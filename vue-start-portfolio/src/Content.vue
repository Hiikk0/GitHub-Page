<template>
  <div :class="['content', className]"></div>
</template>

<script>
export default {
  name: "Content",
  props: {
    className: {
      type: String,
      default: ""
    }
  }
};
</script>

<style>
.content {
  height: 833px;
  position: relative;
  width: 100%;
  max-width: 1420px;
  margin: 0 auto; 
}
</style>