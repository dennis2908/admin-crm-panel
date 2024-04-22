<template>
  <div :class="$style.errorHandlerInner"><Frame1 /></div>
</template>
<script>
  import { defineComponent } from "vue";
  import Frame1 from "./Frame1.vue";

  export default defineComponent({
    name: "Frame",
    components: { Frame1 },
  });
</script>
<style module>
  .errorHandlerInner {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-336xl);
    box-sizing: border-box;
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-5xl);
    color: var(--color-white);
    font-family: var(--font-poppins);
  }

  @media screen and (max-width: 1250px) {
    .errorHandlerInner {
      padding-left: var(--padding-158xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 825px) {
    .errorHandlerInner {
      padding-left: var(--padding-69xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 450px) {
    .errorHandlerInner {
      padding-left: var(--padding-xl);
      box-sizing: border-box;
    }
  }
</style>