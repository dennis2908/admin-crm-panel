<template>
  <div :class="$style.mobile">
    <FunctionTree />
    <section :class="$style.rectangleParent">
      <div :class="$style.frameChild" />
      <Frame4 />
      <div :class="$style.frameWrapper">
        <div :class="$style.frameParent">
          <div :class="$style.frameGroup">
            <div :class="$style.parent">
              <div :class="$style.div">상호명</div>
              <div :class="$style.div1">하이퍼하이어</div>
            </div>
            <div :class="$style.ceoParent">
              <div :class="$style.ceo">대표 CEO</div>
              <div :class="$style.div2">김주현</div>
            </div>
          </div>
          <div :class="$style.hyperhireIndiaPrivateLimiteParent">
            <div :class="$style.hyperhireIndiaPrivate">
              Hyperhire India Private Limited
            </div>
            <div :class="$style.juhyunKimWrapper">
              <div :class="$style.juhyunKim">Juhyun Kim</div>
            </div>
          </div>
        </div>
      </div>
      <div :class="$style.cinParent">
        <div :class="$style.cin">사업자등록번호 CIN</div>
        <div :class="$style.group">
          <div :class="$style.div3">427-86-01187</div>
          <div :class="$style.u74110dl2016ptc290812">U74110DL2016PTC290812</div>
        </div>
      </div>
      <Frame3 />
    </section>
  </div>
</template>
<script>
  import { defineComponent } from "vue";
  import FunctionTree from "../components/FunctionTree.vue";
  import Frame4 from "../components/Frame4.vue";
  import Frame3 from "../components/Frame3.vue";

  export default defineComponent({
    name: "Mobile",
    components: { FunctionTree, Frame4, Frame3 },
  });
</script>
<style module>
  .frameChild {
    width: 100%;
    height: 100%;
    position: absolute;
    margin: 0 !important;
    top: 1063px;
    right: -360px;
    bottom: -1063px;
    left: 360px;
    background-color: var(--color-gray-100);
    transform: rotate(180deg);
    transform-origin: 0 0;
  }
  .div {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 36px;
    z-index: 1;
  }
  .div1 {
    position: relative;
    font-size: var(--font-size-smi);
    line-height: 20px;
    font-weight: 900;
    color: var(--blue-gray-60);
    display: inline-block;
    min-width: 78px;
    z-index: 1;
  }
  .parent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-3xs);
  }
  .ceo {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 52px;
    z-index: 1;
  }
  .div2 {
    position: relative;
    font-size: var(--font-size-smi);
    line-height: 20px;
    font-weight: 900;
    color: var(--blue-gray-60);
    display: inline-block;
    min-width: 39px;
    z-index: 1;
  }
  .ceoParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-3xs);
  }
  .frameGroup {
    width: 275px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    padding: 0px var(--padding-xl) 0px 0px;
    box-sizing: border-box;
    gap: var(--gap-xl);
  }
  .hyperhireIndiaPrivate {
    position: relative;
    line-height: 20px;
    font-weight: 900;
    z-index: 1;
  }
  .juhyunKim {
    position: relative;
    line-height: 20px;
    font-weight: 900;
    display: inline-block;
    min-width: 83px;
    z-index: 2;
  }
  .juhyunKimWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-10xs) 0px 0px;
    margin-left: -9px;
  }
  .hyperhireIndiaPrivateLimiteParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
  }
  .frameParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-8xs);
  }
  .frameWrapper {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs);
  }
  .cin {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 109px;
    z-index: 1;
  }
  .div3 {
    position: relative;
    line-height: 20px;
    font-weight: 900;
    display: inline-block;
    min-width: 90px;
    z-index: 1;
  }
  .u74110dl2016ptc290812 {
    position: relative;
    line-height: 20px;
    font-weight: 900;
    z-index: 1;
  }
  .group {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-8xs);
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
  }
  .cinParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-xl) 0px 0px;
    gap: var(--gap-3xs);
  }
  .rectangleParent {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 64px var(--padding-base) var(--padding-41xl);
    box-sizing: border-box;
    position: relative;
    gap: var(--gap-17xl);
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-xs);
    color: var(--blue-gray-80);
    font-family: var(--font-poppins);
  }
  .mobile {
    width: 100%;
    position: relative;
    background-color: var(--color-white);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    line-height: normal;
    letter-spacing: normal;
  }
</style>