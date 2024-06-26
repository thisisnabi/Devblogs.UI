<template>
  <div class="mt-5 pt-5">
    <dashed-title classList="font-demi mt-3" dashedSide="both">
      سرفصل های دوره
    </dashed-title>

    <div class="row mt-5 align-items-start">
      <div class="col-9">
        <accordion></accordion>
      </div>
      <aside class="col-3 sticky-top sidebar px-1">
        <div class="price-box d-flex flex-column p-4 align-items-center">
          <p class="mb-2 p-size-big font-med">
            قیمت دوره
          </p>
          <del class="opacity-600 mb-3">
            ۷،۹۰۰،۰۰۰ تومان
          </del>
          <span class="mb-3 h3-size font-demi">
            ۷،۸۰۰،۰۰۰
            <span class="p-size">
              تومان
            </span>
          </span>
          <btn classList="w-100 font-bold p-size-big">خرید دوره</btn>
        </div>
      </aside>
    </div>

  </div>
</template>

<script>
import Btn from '../particles/btn.vue'
import Accordion from '../particles/accordion.vue'
import dashedTitle from '../particles/dashedTitle.vue'
export default {
  components: { dashedTitle, Accordion, Btn },
}
</script>

<style lang="scss" scoped>
.sidebar{
  top: 140px;
  .price-box{
    background: $bg-color;
    border-radius: 16px;
  }
}
</style>
