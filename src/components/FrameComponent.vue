<template>
  <button :class="$style.frameParent">
    <div :class="$style.iconImageWrapper">
      <img :class="$style.iconImage" alt="" :src="iconImage" />
    </div>
    <div :class="$style.wrapper">
      <div :class="$style.div">{{prop}}</div>
    </div>
  </button>
</template>
<script>
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "FrameComponent",
    props: {
      iconImage: { type: String },
      prop: { type: String },
    },
  });
</script>
<style module>
  .iconImage {
    height: 32px;
    width: 32px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .iconImageWrapper {
    border-radius: var(--br-5xs);
    background-color: var(--color-gray-400);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-xs);
  }
  .div {
    align-self: stretch;
    position: relative;
    font-size: var(--font-size-5xl);
    line-height: 150%;
    font-weight: 900;
    font-family: var(--font-poppins);
    color: var(--color-white);
    text-align: left;
  }
  .wrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-9xs) 0px 0px;
    box-sizing: border-box;
    min-width: 143px;
  }
  .frameParent {
    cursor: pointer;
    border: none;
    padding: var(--padding-base);
    background-color: var(--color-gray-500);
    flex: 1;
    border-radius: var(--br-xs);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    box-sizing: border-box;
    gap: var(--gap-5xl);
    min-width: 137px;
    max-width: 100%;
  }

  @media screen and (max-width: 450px) {
    .div {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .frameParent {
      flex-wrap: wrap;
    }
  }
</style>