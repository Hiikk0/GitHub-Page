<template>
  <div :class="['header', className]">
    <div class="text-and-icon">
      <img class="icon" alt="Icon" :src="icon" />
      <div class="text-wrapper">Hikko</div>
    </div>

    <img class="horizontal" alt="Horizontal" :src="horizontalDecorationLine" />

    <div class="navigation">
      <div class="div">Home</div>

      <img
        class="vertical-decoration"
        alt="Vertical decoration"
        :src="verticalDecorationLine"
      />

      <div class="div">About me</div>

      <img
        class="vertical-decoration"
        alt="Vertical decoration"
        :src="verticalDecorationLine"
      />

      <div class="div">My projects</div>

      <img
        class="vertical-decoration"
        alt="Vertical decoration"
        :src="verticalDecorationLine"
      />

      <div class="div">Contacts</div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import horizontalDecorationLine from "@/assets/horizontal-decoration-line.svg";
import icon from "@/assets/icon.png";
import verticalDecorationLine from "@/assets/vertical-decoration-line.svg";

export default defineComponent({
  name: "Header",
  props: {
    className: {
      type: String,
      default: "",
    },
  },
  data() {
    return {
      horizontalDecorationLine,
      icon,
      verticalDecorationLine,
    };
  },
});
</script>

<style>
.header {
  align-items: center;
  display: flex;
  gap: 10px;
  justify-content: center;
  padding: 10px;
  position: relative;
  width: 100%;
  max-width: 1420px;
  margin: 0 auto;
}

.header .text-and-icon {
  align-items: center;
  display: inline-flex;
  flex: 0 0 auto;
  gap: 10px;
  position: relative;
}

.header .icon {
  height: 48px;
  object-fit: cover;
  position: relative;
  width: 48px;
}

.header .text-wrapper {
  align-items: center;
  color: #000000;
  display: flex;
  font-family: "Allerta Stencil-Regular", Helvetica;
  font-size: 48px;
  font-weight: 400;
  justify-content: center;
  letter-spacing: 0;
  line-height: normal;
  position: relative;
  white-space: nowrap;
  width: fit-content;
}

.header .horizontal {
  flex: 1;
  flex-grow: 1;
  height: 1.7px;
  object-fit: cover;
  position: relative;
}

.header .navigation {
  align-items: center;
  display: inline-flex;
  flex: 0 0 auto;
  gap: 10px;
  justify-content: center;
  padding: 10px;
  position: relative;
}

.header .div {
  align-items: center;
  color: #000000;
  display: flex;
  font-family: "Allerta Stencil-Regular", Helvetica;
  font-size: 24px;
  font-weight: 400;
  justify-content: center;
  letter-spacing: 0;
  line-height: normal;
  position: relative;
  white-space: nowrap;
  width: fit-content;
}

.header .vertical-decoration {
  height: 31.06px;
  position: relative;
  width: auto;
}
</style>