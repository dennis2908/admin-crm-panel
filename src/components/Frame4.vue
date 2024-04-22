<template>
  <div :class="$style.parent">
    <img :class="$style.icon" loading="lazy" alt="" src="/-11.svg" />
    <div :class="$style.div">
      우리는 국가의 장벽을 넘어 최고의 인재를 매칭해드립니다.
    </div>
    <div :class="$style.inputFilterParent">
      <div :class="$style.inputFilter">010-0000-0000</div>
      <div :class="$style.aaaaanavercom">aaaaa@naver.com</div>
    </div>
    <div :class="$style.outputCombiner">
      <div :class="$style.instanceParent">
        <div :class="$style.frameParent">
          <div :class="$style.frameGroup">
            <div :class="$style.frameWrapper">
              <img
                :class="$style.frameChild"
                loading="lazy"
                alt=""
                src="/frame-5041.svg"
              />
            </div>
            <div :class="$style.wrapper">
              <div :class="$style.div1">
                <p :class="$style.p">해외 개발자 원격 채용</p>
              </div>
            </div>
          </div>
          <div :class="$style.group">
            <div :class="$style.div2">바로가기</div>
            <img
              :class="$style.iconlylightOutlinearrowR"
              loading="lazy"
              alt=""
              src="/iconlylightoutlinearrow--right-square1@2x.png"
            />
          </div>
        </div>
        <div :class="$style.frameContainer">
          <div :class="$style.frameDiv">
            <div :class="$style.korWrapper">
              <b :class="$style.kor">KOR</b>
            </div>
            <div :class="$style.container">
              <div :class="$style.div3">한국어 가능 외국인 채용</div>
            </div>
          </div>
          <div :class="$style.parent1">
            <div :class="$style.div4">바로가기</div>
            <img
              :class="$style.iconlylightOutlinearrowR1"
              loading="lazy"
              alt=""
              src="/iconlylightoutlinearrow--right-square-1@2x.png"
            />
          </div>
        </div>
      </div>
      <div :class="$style.frameParent1">
        <div :class="$style.frameParent2">
          <div :class="$style.frameParent3">
            <div :class="$style.frameWrapper1">
              <img
                :class="$style.frameItem"
                loading="lazy"
                alt=""
                src="/frame-5041-1.svg"
              />
            </div>
            <div :class="$style.frame">
              <div :class="$style.div5">
                <p :class="$style.p1">외국인 원격 채용</p>
                <p :class="$style.p2">(비개발)</p>
              </div>
            </div>
          </div>
          <div :class="$style.parent2">
            <div :class="$style.div6">바로가기</div>
            <img
              :class="$style.iconlylightOutlinearrowR2"
              loading="lazy"
              alt=""
              src="/iconlylightoutlinearrow--right-square-2@2x.png"
            />
          </div>
        </div>
        <FrameInstance
          iconCode="/setting-1.svg"
          prop1="해외 개발자 활용 서비스"
          iconlyLightOutlineArrowRi="/iconlylightoutlinearrow--right-square@2x.png"
          propFlex="unset"
          propPadding="var(--padding-base) var(--padding-5xs) var(--padding-base) var(--padding-base)"
          frameDivMinWidth="unset"
          frameDivAlignSelf="stretch"
          frameDivAlignSelf1="stretch"
          divDisplay="unset"
          divMinWidth="unset"
        />
      </div>
    </div>
  </div>
</template>
<script>
  import { defineComponent } from "vue";
  import FrameInstance from "./FrameInstance.vue";

  export default defineComponent({
    name: "Frame4",
    components: { FrameInstance },
  });
</script>
<style module>
  .icon {
    width: 187px;
    height: 34px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
    z-index: 1;
  }
  .div {
    width: 247px;
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    z-index: 1;
  }
  .inputFilter {
    position: relative;
    line-height: 20px;
    font-weight: 900;
    display: inline-block;
    min-width: 107px;
    z-index: 1;
  }
  .aaaaanavercom {
    position: relative;
    line-height: 20px;
    font-weight: 900;
    white-space: nowrap;
    z-index: 1;
  }
  .inputFilterParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-xl) 0px 0px;
    gap: var(--gap-5xs);
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
  }
  .frameChild {
    width: 24px;
    height: 24px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .frameWrapper {
    border-radius: var(--br-5xs);
    background-color: var(--color-ghostwhite);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs);
  }
  .p {
    margin: 0;
  }
  .div1 {
    position: relative;
    line-height: 150%;
    font-weight: 900;
  }
  .wrapper {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .frameGroup {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-xs);
  }
  .div2 {
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
  .group {
    width: 76px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    color: var(--blue-gray-60);
  }
  .frameParent {
    align-self: stretch;
    border-radius: var(--br-xs);
    background-color: var(--color-white);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-base) var(--padding-xl) var(--padding-base)
      var(--padding-base);
    gap: var(--gap-base);
    z-index: 1;
  }
  .kor {
    height: 24px;
    position: relative;
    line-height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    min-width: 24px;
  }
  .korWrapper {
    border-radius: var(--br-5xs);
    background-color: var(--color-ghostwhite);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs);
  }
  .div3 {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    white-space: nowrap;
  }
  .container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    text-align: left;
    font-size: var(--font-size-sm);
    color: var(--blue-gray-80);
    font-family: var(--font-poppins);
  }
  .frameDiv {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-xs);
  }
  .div4 {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 900;
  }
  .iconlylightOutlinearrowR1 {
    height: 20px;
    width: 20px;
    position: relative;
    object-fit: cover;
  }
  .parent1 {
    width: 76px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    text-align: left;
    font-size: var(--font-size-sm);
    color: var(--blue-gray-60);
    font-family: var(--font-poppins);
  }
  .frameContainer {
    align-self: stretch;
    border-radius: var(--br-xs);
    background-color: var(--color-white);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-base) var(--padding-5xs) var(--padding-base)
      var(--padding-base);
    gap: var(--gap-base);
    z-index: 1;
    text-align: center;
    font-size: var(--font-size-xs-2);
    color: var(--color-lightslategray-200);
    font-family: var(--font-nunito);
  }
  .instanceParent {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .frameItem {
    width: 24px;
    height: 24px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .frameWrapper1 {
    border-radius: var(--br-5xs);
    background-color: var(--color-ghostwhite);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs);
  }
  .p1 {
    margin: 0;
  }
  .p2 {
    margin: 0;
  }
  .div5 {
    height: 42px;
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
  }
  .frame {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .frameParent3 {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-xs);
  }
  .div6 {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 900;
  }
  .iconlylightOutlinearrowR2 {
    height: 20px;
    width: 20px;
    position: relative;
    object-fit: cover;
  }
  .parent2 {
    width: 76px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    color: var(--blue-gray-60);
  }
  .frameParent2 {
    align-self: stretch;
    border-radius: var(--br-xs);
    background-color: var(--color-white);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-base) var(--padding-27xl) var(--padding-base)
      var(--padding-base);
    gap: var(--gap-base);
    z-index: 1;
  }
  .frameParent1 {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .outputCombiner {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .parent {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px var(--padding-5xl);
    gap: var(--gap-mid-3);
    text-align: left;
    font-size: var(--font-size-sm);
    color: var(--blue-gray-80);
    font-family: var(--font-poppins);
  }
</style>