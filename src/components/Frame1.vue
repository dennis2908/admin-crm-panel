<template>
  <div :class="$style.frameParent">
    <Frame2
      iconMarketing="/iconmarketing.svg"
      prop="해외 마케팅"
    /><FrameComponent
      iconImage="/iconimage.svg"
      prop="퍼블리셔"
    /><FrameComponent iconImage="/iconbox.svg" prop="캐드원(제도사)" /><Frame2
      iconMarketing="/icontarget.svg"
      prop="해외 세일즈"
      propOverflow="unset"
      propPadding="0px var(--padding-9xs) 0px 0px"
    /><Frame2
      iconMarketing="/iconcall.svg"
      prop="해외 CS"
      propOverflow="hidden"
      propPadding="unset"
    />
    <div :class="$style.frameGroup">
      <div :class="$style.presentationWrapper">
        <img
          :class="$style.presentationIcon"
          loading="lazy"
          alt=""
          src="/iconmarketing.svg"
        />
      </div>
      <div :class="$style.wrapper">
        <h2 :class="$style.h2">해외 마케팅</h2>
      </div>
    </div>
  </div>
</template>
<script>
  import { defineComponent } from "vue";
  import Frame2 from "./Frame2.vue";
  import FrameComponent from "./FrameComponent.vue";

  export default defineComponent({
    name: "Frame1",
    components: { Frame2, FrameComponent },
  });
</script>
<style module>
  .presentationIcon {
    height: 32px;
    width: 32px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .presentationWrapper {
    border-radius: var(--br-5xs);
    background-color: var(--color-gray-400);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-xs);
  }
  .h2 {
    margin: 0;
    align-self: stretch;
    height: 36px;
    position: relative;
    font-size: inherit;
    line-height: 150%;
    font-weight: 900;
    font-family: inherit;
    display: inline-block;
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
  .frameGroup {
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
  }
  .frameParent {
    width: 2042px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-9xs) 0px 0px;
    box-sizing: border-box;
    gap: 10px 9.2px;
    max-width: 131%;
    flex-shrink: 0;
    z-index: 2;
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

    .frameGroup {
      flex-wrap: wrap;
    }
  }
</style>