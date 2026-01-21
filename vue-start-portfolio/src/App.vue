<template>
  <div class="desktop">
    <Header class="header-instance" />
    <Content class="content-instance" />
    <Footer class="footer-instance" />
  </div>
</template>

<script>
import Header from "./Header.vue";
import Content from "./Content.vue";
import Footer from "./Footer.vue";

export default {
  name: "Desktop",
  components: {
    Header,
    Content,
    Footer,
  },
};
</script>

<style>
  @font-face {
  font-family: "Allerta Stencil-Regular"; /* Це ім'я ви будете використовувати далі */
  src: url("@/assets/fonts/AllertaStencil-Regular.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}
.desktop {
  align-items: flex-start;
  background-color: #ffffff;
  display: flex;
  flex-direction: column;
  gap: 10px;
  min-height: 100vh;
  padding: 10px;
  position: relative;
}

.desktop .header-instance {
  align-self: stretch !important;
  background-color: transparent !important;
  flex: 0 0 auto !important;
  left: unset !important;
  top: unset !important;
  width: 100% !important;
}

.desktop .content-instance {
  align-self: stretch !important;
  flex: 1 !important;
  flex-grow: 1 !important;
  height: unset !important;
  left: unset !important;
  top: unset !important;
  width: 100% !important;
}

.desktop .footer-instance {
  left: unset !important;
  top: unset !important;
}
</style>