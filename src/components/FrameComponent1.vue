<template>
  <section :class="$style.frameParent">
    <div :class="$style.frameWrapper">
      <div :class="$style.fadeInAfterTitleSubtitleParent">
        <div :class="$style.fadeInAfter">
          FadeIn after title and subtitle shown(delay 300ms)
        </div>
        <div :class="$style.functionEntryParent">
          <button :class="$style.functionEntry">
            <div :class="$style.div">풀타임, 파트타임</div>
          </button>
          <div :class="$style.loopCounter">
            <img
              :class="$style.dataMergeIcon"
              loading="lazy"
              alt=""
              src="/polygon-1.svg"
            />
          </div>
        </div>
      </div>
    </div>
    <div :class="$style.eventReceiverParent">
      <button :class="$style.eventReceiver">
        <img :class="$style.eventReceiverChild" alt="" src="/group-5096.svg" />
        <div :class="$style.div1">월 100만원</div>
      </button>
      <div :class="$style.fadeinTooltipsBottomCardWrapper">
        <div :class="$style.fadeinTooltipsBottom">
          FadeIn tooltips, bottom card, and arrows with the title (500ms)
        </div>
      </div>
    </div>
  </section>
</template>
<script>
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "FrameComponent1",
  });
</script>
<style module>
  .fadeInAfter {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    z-index: 2;
  }
  .div {
    position: relative;
    font-size: var(--font-size-lg);
    line-height: 150%;
    font-weight: 900;
    font-family: var(--font-poppins);
    color: var(--color-darkturquoise);
    text-align: left;
    display: inline-block;
    min-width: 126px;
    white-space: nowrap;
  }
  .functionEntry {
    cursor: pointer;
    border: none;
    padding: var(--padding-7xs) var(--padding-xs);
    background-color: var(--color-white);
    position: absolute;
    top: 0px;
    left: 0px;
    border-radius: var(--br-5xs);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    white-space: nowrap;
    z-index: 2;
  }
  .functionEntry:hover {
    background-color: var(--color-gainsboro-100);
  }
  .dataMergeIcon {
    height: 14px;
    width: 14px;
    position: relative;
    border-radius: var(--br-12xs-5);
    object-fit: contain;
  }
  .loopCounter {
    position: absolute;
    top: 34px;
    left: 0px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-3xs);
    z-index: 3;
  }
  .functionEntryParent {
    height: 48px;
    width: 150px;
    position: relative;
  }
  .fadeInAfterTitleSubtitleParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-15xl);
  }
  .frameWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-20xl) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .eventReceiverChild {
    height: 26px;
    width: 26px;
    position: relative;
  }
  .div1 {
    position: relative;
    font-size: var(--font-size-lg);
    line-height: 150%;
    font-weight: 900;
    font-family: var(--font-poppins);
    color: var(--trabuddy-alternative);
    text-align: left;
    display: inline-block;
    min-width: 84px;
  }
  .eventReceiver {
    cursor: pointer;
    border: none;
    padding: var(--padding-5xs) var(--padding-base);
    background-color: var(--nephritis-05);
    border-radius: var(--br-5xs);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-3xs);
    white-space: nowrap;
    z-index: 2;
  }
  .eventReceiver:hover {
    background-color: var(--color-gainsboro-200);
  }
  .fadeinTooltipsBottom {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    z-index: 2;
  }
  .fadeinTooltipsBottomCardWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-4xs) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .eventReceiverParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-54xl-2);
    max-width: 100%;
  }
  .frameParent {
    width: 1680px;
    margin: 0 !important;
    position: absolute;
    top: 249px;
    right: 87px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    max-width: 100%;
    gap: var(--gap-xl);
    text-align: left;
    font-size: var(--font-size-3xs);
    color: var(--yellow-40);
    font-family: var(--font-poppins);
  }

  @media screen and (max-width: 1550px) {
    .frameParent {
      flex-wrap: wrap;
    }
  }
  @media screen and (max-width: 825px) {
    .fadeInAfterTitleSubtitleParent {
      flex-wrap: wrap;
    }

    .eventReceiverParent {
      flex-wrap: wrap;
    }
  }
</style>