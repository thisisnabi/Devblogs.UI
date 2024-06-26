<template>
  <div class="coming-soon d-flex flex-column align-items-center justify-content-center pt-5 mt-5">
    <h2 class="text-center h1-size font-bold pb-4">
      بزودی برگزار می شود...
    </h2>
    <img width="400px" loading="lazy" src="/img/design/empty-gallery.png" alt="empty-gallery" />
    <svg width="926" height="926" viewBox="0 0 926 926" fill="none" xmlns="http://www.w3.org/2000/svg">
      <g opacity="0.3" filter="url(#filter0_f_1_5357)">
      <circle cx="463" cy="463" r="163" fill="#8C6DED"/>
      </g>
      <defs>
      <filter id="filter0_f_1_5357" x="0" y="0" width="926" height="926" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
      <feFlood flood-opacity="0" result="BackgroundImageFix"/>
      <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
      <feGaussianBlur stdDeviation="150" result="effect1_foregroundBlur_1_5357"/>
      </filter>
      </defs>
    </svg>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.coming-soon{
  position: relative;
  svg{
    position: absolute;
    z-index: -1;
    opacity: .8;
  }
}
</style>
