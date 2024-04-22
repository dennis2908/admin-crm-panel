<template>
  <div :class="$style.frameParent" :style="frameDiv1Style">
    <div :class="$style.frameGroup" :style="frameDiv2Style">
      <div :class="$style.iconCodeWrapper">
        <img :class="$style.iconCode" loading="lazy" alt="" :src="iconCode" />
      </div>
      <div :class="$style.wrapper">
        <div :class="$style.div" :style="divStyle">{{prop1}}</div>
      </div>
    </div>
    <div :class="$style.parent">
      <div :class="$style.div1">바로가기</div>
      <img
        :class="$style.iconlylightOutlinearrowR"
        loading="lazy"
        alt=""
        :src="iconlyLightOutlineArrowRi"
      />
    </div>
  </div>
</template>
<script>
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "FrameInstance",
    props: {
      iconCode: { type: String },
      prop1: { type: String },
      iconlyLightOutlineArrowRi: { type: String },
      propFlex: { type: String },
      propPadding: { type: [Object, Array, String, Number, Boolean] },
      frameDivMinWidth: { type: [Object, Array, String, Number, Boolean] },
      frameDivAlignSelf: { type: String },
      frameDivAlignSelf1: { type: String },
      divDisplay: { type: String },
      divMinWidth: { type: [Object, Array, String, Number, Boolean] },
    },
    computed: {
      frameDiv1Style() {
        return {
          flex: this.propFlex,
          padding: this.propPadding,
          minWidth: this.frameDivMinWidth,
          alignSelf: this.frameDivAlignSelf,
        };
      },
      frameDiv2Style() {
        return {
          alignSelf: this.frameDivAlignSelf1,
        };
      },
      divStyle() {
        return {
          display: this.divDisplay,
          minWidth: this.divMinWidth,
        };
      },
    },
  });
</script>
<style module>
  .iconCode {
    width: 24px;
    height: 24px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .iconCodeWrapper {
    border-radius: var(--br-5xs);
    background-color: var(--color-ghostwhite);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs);
  }
  .div {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 124px;
    white-space: nowrap;
  }
  .wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .frameGroup {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-xs);
  }
  .div1 {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 900;
  }
  .iconlylightOutlinearrowR {
    height: 20px;
    width: 20px;
    position: relative;
    object-fit: cover;
  }
  .parent {
    width: 76px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    color: var(--blue-gray-60);
  }
  .frameParent {
    border-radius: var(--br-xs);
    background-color: var(--color-white);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-base) var(--padding-28xl) var(--padding-base)
      var(--padding-base);
    gap: var(--gap-base);
    z-index: 1;
    text-align: left;
    font-size: var(--font-size-sm);
    color: var(--blue-gray-80);
    font-family: var(--font-poppins);
  }
</style>