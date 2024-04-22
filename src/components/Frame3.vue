<template>
  <div :class="$style.frameParent">
    <div :class="$style.addressWrapper">
      <div :class="$style.address">주소 ADDRESS</div>
    </div>
    <div :class="$style.wrapper">
      <div :class="$style.div">서울특별시 강남대로 479, 지하 1층 238호</div>
    </div>
    <footer :class="$style.d138StreetNumber11JagjeWrapper">
      <div :class="$style.d138StreetNumberContainer">
        <p :class="$style.d138StreetNumber">
          D-138, Street number 11, Jagjeet Nagar, North East Delhi, New Delhi,
        </p>
        <p :class="$style.india">110053 India</p>
      </div>
    </footer>
    <div :class="$style.hyperhire">ⓒ 2023 Hyperhire</div>
  </div>
</template>
<script>
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "Frame3",
  });
</script>
<style module>
  .address {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 83px;
    z-index: 1;
  }
  .addressWrapper {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs) var(--padding-8xs);
    font-size: var(--font-size-xs);
    color: var(--blue-gray-80);
  }
  .div {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 900;
    white-space: nowrap;
    z-index: 1;
  }
  .wrapper {
    width: 226px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs);
    box-sizing: border-box;
  }
  .d138StreetNumber {
    margin: 0;
  }
  .india {
    margin: 0;
  }
  .d138StreetNumberContainer {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    max-width: 100%;
    z-index: 1;
  }
  .d138StreetNumber11JagjeWrapper {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px var(--padding-12xl) var(--padding-12xs);
    box-sizing: border-box;
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
    font-family: var(--font-poppins);
  }
  .hyperhire {
    position: relative;
    line-height: 20px;
    font-weight: 900;
    display: inline-block;
    min-width: 118px;
    z-index: 1;
  }
  .frameParent {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-8xs);
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-smi);
    color: var(--blue-gray-60);
    font-family: var(--font-poppins);
  }
</style>