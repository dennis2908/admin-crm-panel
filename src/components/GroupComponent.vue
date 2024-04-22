<template>
  <footer :class="$style.rectangleParent">
    <div :class="$style.frameChild" />
    <div :class="$style.characterCreator">
      <div :class="$style.parent">
        <img :class="$style.icon" loading="lazy" alt="" src="/-1.svg" />
        <div :class="$style.div">
          우리는 국가의 장벽을 넘어 최고의 인재를 매칭해드립니다.
        </div>
        <div :class="$style.group">
          <div :class="$style.div1">010-0000-0000</div>
          <div :class="$style.aaaaanavercom">aaaaa@naver.com</div>
        </div>
      </div>
      <div :class="$style.characterCreatorInner">
        <div :class="$style.frameParent">
          <div :class="$style.frameGroup">
            <div :class="$style.container">
              <div :class="$style.div2">상호명</div>
              <div :class="$style.div3">하이퍼하이어</div>
            </div>
            <div :class="$style.ceoParent">
              <div :class="$style.ceo">대표 CEO</div>
              <div :class="$style.div4">김주현</div>
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
      <div :class="$style.hyperhire">ⓒ 2023 Hyperhire</div>
    </div>
    <div :class="$style.frameContainer">
      <div :class="$style.instanceParent">
        <FrameInstance
          iconCode="/iconcode.svg"
          prop1="해외 개발자 원격 채용"
          iconlyLightOutlineArrowRi="/iconlylightoutlinearrow--right-square@2x.png"
        />
        <div :class="$style.cinParent">
          <div :class="$style.cin">사업자등록번호 CIN</div>
          <div :class="$style.frameDiv">
            <div :class="$style.div5">427-86-01187</div>
            <div :class="$style.u74110dl2016ptc290812">
              U74110DL2016PTC290812
            </div>
          </div>
        </div>
      </div>
      <div :class="$style.linkConnector">
        <div :class="$style.dataProcessorParent">
          <FrameInstance
            iconCode="/iconavatar.svg"
            prop1="외국인 원격 채용 (비개발)"
            iconlyLightOutlineArrowRi="/iconlylightoutlinearrow--right-square@2x.png"
            propFlex="1"
            propPadding="var(--padding-base) var(--padding-3xl) var(--padding-base) var(--padding-base)"
            frameDivMinWidth="140px"
            frameDivAlignSelf="unset"
            frameDivAlignSelf1="stretch"
            divDisplay="unset"
            divMinWidth="unset"
          /><FrameInstance
            iconCode="/iconkor.svg"
            prop1="한국어 가능 외국인 채용"
            iconlyLightOutlineArrowRi="/iconlylightoutlinearrow--right-square@2x.png"
            propFlex="0.9128"
            propPadding="var(--padding-base) var(--padding-16xl) var(--padding-base) var(--padding-base)"
            frameDivMinWidth="140px"
            frameDivAlignSelf="unset"
            frameDivAlignSelf1="stretch"
            divDisplay="unset"
            divMinWidth="unset"
          /><FrameInstance
            iconCode="/icongear.svg"
            prop1="해외 개발자 활용 서비스"
            iconlyLightOutlineArrowRi="/iconlylightoutlinearrow--right-square@2x.png"
            propFlex="0.9128"
            propPadding="var(--padding-base) var(--padding-16xl) var(--padding-base) var(--padding-base)"
            frameDivMinWidth="140px"
            frameDivAlignSelf="unset"
            frameDivAlignSelf1="stretch"
            divDisplay="unset"
            divMinWidth="unset"
          />
        </div>
        <div :class="$style.dataAggregatorWrapper">
          <div :class="$style.dataAggregator">
            <div :class="$style.address">주소 ADDRESS</div>
            <div :class="$style.parent1">
              <div :class="$style.div6">
                서울특별시 강남대로 479, 지하 1층 238호
              </div>
              <div :class="$style.d138StreetNumberContainer">
                <p :class="$style.d138StreetNumber">
                  D-138, Street number 11, Jagjeet Nagar, North East Delhi, New
                  Delhi,
                </p>
                <p :class="$style.india">110053 India</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
  import { defineComponent } from "vue";
  import FrameInstance from "./FrameInstance.vue";

  export default defineComponent({
    name: "GroupComponent",
    components: { FrameInstance },
  });
</script>
<style module>
  .frameChild {
    height: 100%;
    width: 100%;
    position: absolute;
    margin: 0 !important;
    top: 505px;
    right: -1920px;
    bottom: -505px;
    left: 1920px;
    background-color: var(--color-gray-100);
    transform: rotate(180deg);
    transform-origin: 0 0;
  }
  .icon {
    width: 187px;
    height: 34px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
    z-index: 1;
  }
  .div {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 900;
    z-index: 1;
  }
  .div1 {
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
  .group {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
  }
  .parent {
    width: 247px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-mid);
  }
  .div2 {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 36px;
    z-index: 1;
  }
  .div3 {
    position: relative;
    font-size: var(--font-size-smi);
    line-height: 20px;
    font-weight: 900;
    color: var(--blue-gray-60);
    display: inline-block;
    min-width: 78px;
    z-index: 1;
  }
  .container {
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
  .div4 {
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
    width: 255px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
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
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    row-gap: 20px;
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
  }
  .frameParent {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-8xs);
  }
  .characterCreatorInner {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-12xs);
    font-size: var(--font-size-xs);
  }
  .hyperhire {
    position: relative;
    font-size: var(--font-size-smi);
    line-height: 20px;
    font-weight: 900;
    color: var(--blue-gray-60);
    display: inline-block;
    min-width: 118px;
    z-index: 1;
  }
  .characterCreator {
    width: 287px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-26xl-5);
    min-width: 287px;
  }
  .cin {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 109px;
    z-index: 1;
  }
  .div5 {
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
  .frameDiv {
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
    gap: var(--gap-3xs);
    font-size: var(--font-size-xs);
  }
  .instanceParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-43xl);
  }
  .dataProcessorParent {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-base);
  }
  .address {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 83px;
    z-index: 1;
  }
  .div6 {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    white-space: nowrap;
    z-index: 1;
  }
  .d138StreetNumber {
    margin: 0;
  }
  .india {
    margin: 0;
  }
  .d138StreetNumberContainer {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    z-index: 1;
  }
  .parent1 {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-8xs);
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
  }
  .dataAggregator {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-3xs);
    max-width: 100%;
  }
  .dataAggregatorWrapper {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs);
    box-sizing: border-box;
    max-width: 100%;
  }
  .linkConnector {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-43xl);
    min-width: 385px;
    max-width: 100%;
    font-size: var(--font-size-xs);
  }
  .frameContainer {
    flex: 1;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-mini);
    min-width: 517px;
    max-width: 100%;
  }
  .rectangleParent {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-61xl) var(--padding-341xl);
    box-sizing: border-box;
    position: relative;
    gap: var(--gap-99xl);
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-sm);
    color: var(--blue-gray-80);
    font-family: var(--font-poppins);
  }

  @media screen and (max-width: 1550px) {
    .characterCreator {
      flex: 1;
    }

    .frameContainer {
      min-width: 100%;
    }

    .rectangleParent {
      flex-wrap: wrap;
    }
  }
  @media screen and (max-width: 1250px) {
    .linkConnector {
      min-width: 100%;
    }

    .frameContainer {
      flex-wrap: wrap;
    }

    .rectangleParent {
      gap: var(--gap-40xl);
      padding-left: var(--padding-161xl);
      padding-right: var(--padding-161xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 825px) {
    .dataProcessorParent {
      flex-wrap: wrap;
    }

    .linkConnector {
      gap: var(--gap-12xl);
    }

    .rectangleParent {
      gap: var(--gap-10xl);
      padding: var(--padding-33xl) var(--padding-71xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 450px) {
    .juhyunKimWrapper {
      margin-left: 0;
    }

    .hyperhireIndiaPrivateLimiteParent {
      flex-wrap: wrap;
    }

    .characterCreator {
      gap: var(--gap-4xl);
    }

    .linkConnector {
      gap: var(--gap-mini);
    }
  }
</style>