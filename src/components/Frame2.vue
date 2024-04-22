<template>
  <div :class="$style.frameParent">
    <button :class="$style.iconMarketingWrapper">
      <img
        :class="$style.iconMarketing"
        alt=""
        :src="iconMarketing"
        :style="iconMarketingStyle"
      />
    </button>
    <div :class="$style.wrapper" :style="frameDivStyle">
      <h2 :class="$style.h2">{{prop}}</h2>
    </div>
  </div>
</template>
<script>
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "Frame2",
    props: {
      iconMarketing: { type: String },
      prop: { type: String },
      propOverflow: { type: String },
      propPadding: { type: [Object, Array, String, Number, Boolean] },
    },
    computed: {
      iconMarketingStyle() {
        return {
          overflow: this.propOverflow,
        };
      },
      frameDivStyle() {
        return {
          padding: this.propPadding,
        };
      },
    },
  });
</script>
<style module>
  .iconMarketing {
    height: 32px;
    width: 32px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .iconMarketingWrapper {
    cursor: pointer;
    border: none;
    padding: var(--padding-xs);
    background-color: var(--color-gray-400);
    border-radius: var(--br-5xs);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .h2 {
    margin: 0;
    align-self: stretch;
    position: relative;
    font-size: inherit;
    line-height: 150%;
    font-weight: 900;
    font-family: inherit;
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
    flex: 1;
    border-radius: var(--br-xs);
    background-color: var(--color-gray-500);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-base);
    box-sizing: border-box;
    gap: var(--gap-5xl);
    min-width: 137px;
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-5xl);
    color: var(--color-white);
    font-family: var(--font-poppins);
  }

  @media screen and (max-width: 450px) {
    .h2 {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .frameParent {
      flex-wrap: wrap;
    }
  }
</style>