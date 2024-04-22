<template>
  <header :class="$style.header">
    <div :class="$style.header1" />
    <div :class="$style.logoWrapper">
      <img :class="$style.logoIcon" loading="lazy" alt="" src="/logo.svg" />
    </div>
    <div :class="$style.menusWrapper">
      <div :class="$style.menus">
        <div :class="$style.dataAggregator">
          <div :class="$style.div">채용</div>
          <div :class="$style.navicaretDownWrapper">
            <img
              :class="$style.navicaretDownIcon"
              alt=""
              src="/navicaretdown.svg"
            />
          </div>
        </div>
        <div :class="$style.div1">해외 개발자 활용 서비스</div>
      </div>
    </div>
    <div :class="$style.btn">
      <div :class="$style.div2">문의하기</div>
    </div>
  </header>
</template>
<script>
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "Header",
  });
</script>
<style module>
  .header1 {
    height: 60px;
    width: 1920px;
    position: relative;
    display: none;
    max-width: 100%;
  }
  .logoIcon {
    align-self: stretch;
    height: 21px;
    position: relative;
    max-width: 100%;
    overflow: hidden;
    flex-shrink: 0;
    z-index: 1;
  }
  .logoWrapper {
    width: 114px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-7xs) 0px 0px;
    box-sizing: border-box;
  }
  .div {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 32px;
  }
  .navicaretDownIcon {
    width: 16px;
    height: 16px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .navicaretDownWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-9xs) 0px 0px;
  }
  .dataAggregator {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-7xs);
  }
  .div1 {
    width: 156px;
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    white-space: nowrap;
  }
  .menus {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    gap: var(--gap-xl);
    z-index: 1;
  }
  .menusWrapper {
    width: 278.5px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-8xs) var(--padding-4xs-5) 0px 0px;
    box-sizing: border-box;
  }
  .div2 {
    position: relative;
    line-height: 150%;
    font-weight: 900;
    display: inline-block;
    min-width: 59px;
  }
  .btn {
    border-radius: var(--br-5xs);
    background-color: var(--color-white);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-7xs) var(--padding-5xl);
    z-index: 1;
    color: var(--color);
  }
  .header {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: var(--padding-smi) var(--padding-xl) var(--padding-2xs)
      var(--padding-2xl);
    box-sizing: border-box;
    gap: var(--gap-332xl);
    max-width: 100%;
    z-index: 2;
    text-align: center;
    font-size: var(--font-size-base);
    color: var(--color-white);
    font-family: var(--font-poppins);
  }

  @media screen and (max-width: 1250px) {
    .header {
      gap: var(--gap-156xl);
    }
  }
  @media screen and (max-width: 825px) {
    .header {
      gap: var(--gap-69xl);
    }
  }
  @media screen and (max-width: 450px) {
    .menus {
      display: none;
    }

    .menusWrapper {
      width: 8.5px;
    }

    .header {
      gap: var(--gap-25xl);
    }
  }
</style>