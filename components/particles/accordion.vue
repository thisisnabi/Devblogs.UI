<template>
  <div class="accordion" role="tablist">
    <b-card v-for="i in 10" :key="i" no-body class="mb-3">
      <b-card-header @click="setActiveTab(i)" header-tag="header" class="p-1" role="tab">
        <b-button v-b-toggle="`accordion-${i}`" block class="d-flex align-items-center justify-content-between">
          <span class="h4-size">
            <svg width="38" height="36" viewBox="0 0 40 38" fill="none" xmlns="http://www.w3.org/2000/svg">
              <g clip-path="url(#clip0_1_7173)">
              <mask id="mask0_1_7173" style="mask-type:luminance" maskUnits="userSpaceOnUse" x="0" y="0" width="40" height="38">
              <path d="M40 0.5H0V37.5H40V0.5Z" fill="white"/>
              </mask>
              <g mask="url(#mask0_1_7173)">
              <mask id="mask1_1_7173" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="5" y="5" width="32" height="30">
              <path fill-rule="evenodd" clip-rule="evenodd" d="M36.6667 5.125H5V34.4167H36.6667V5.125ZM34.1667 15.9167H25.8333V28.25C25.8333 30.3775 27.7 32.1042 30 32.1042C32.3 32.1042 34.1667 30.3775 34.1667 28.25V15.9167Z" fill="#D9D9D9"/>
              </mask>
              <g mask="url(#mask1_1_7173)">
              <path d="M30 32.1041H10.8334C8.53335 32.1041 6.66669 30.3775 6.66669 28.25V6.66663H25.8334V15.9166L30 32.1041Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
              </g>
              <path d="M25.8333 15.9166H34.1666V28.25C34.1666 30.3775 32.3 32.1041 30 32.1041C27.7 32.1041 25.8333 30.3775 25.8333 28.25V15.9166Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
              <path d="M20.8334 11.2916H11.6667V16.6875H20.8334V11.2916Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
              <path d="M11.6667 21.3125H20.8334" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
              <path d="M11.6667 26.0302H20.8334" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
              </g>
              </g>
              <defs>
              <clipPath id="clip0_1_7173">
              <rect width="40" height="37" fill="white" transform="translate(0 0.5)"/>
              </clipPath>
              </defs>
            </svg>
            <span class="font-bold counter pl-4 ml-2 pr-2">
              {{ i }}
            </span>
            restful api در عمل
          </span>
          <span>
            <span class="p-size-big opacity-700 pl-3">
              ۴ ساعت
              <svg width="23" height="23" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M14 6.99992V13.9999L18.6667 16.3333M25.6667 13.9999C25.6667 20.4432 20.4433 25.6666 14 25.6666C7.55668 25.6666 2.33333 20.4432 2.33333 13.9999C2.33333 7.5566 7.55668 2.33325 14 2.33325C20.4433 2.33325 25.6667 7.5566 25.6667 13.9999Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </span>
            <span :class="[activeIndex === i ? 'rotate' : '' , ' arrow']">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M8 11L12 7L16 11M8 17L12 13L16 17" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </span>
          </span>
        </b-button>
      </b-card-header>
      <b-collapse :id="`accordion-${i}`" :visible="i == 1" accordion="my-accordion" role="tabpanel">
        <b-card-body class="p-0 mx-4">
          <div class="acc-desc p-4 mt-1">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است، و برای شرایط فعلی تکنولوژی مورد نیاز، و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد،
            <ul class="mt-3 px-4">
              <li v-for="i in 3" :key="i">
                لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ،
              </li>
            </ul>
          </div>
        </b-card-body>
      </b-collapse>
    </b-card>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: 1
      }
    },
    methods:{
      setActiveTab(i){
        this.activeIndex = i
      }
    }
  }
</script>

<style lang="scss" scoped>
.accordion{
  .rotate svg{
    transform: rotate(180deg);
  }
  .card{
    background: transparent;
    border: 0;
  }
  .acc-desc{
    background: $bg-color;
    line-height: $h2-size;
    color: $light-700;
    *{
      line-height: $h2-size;
      color: $light-700;
    }
  }
  .card-header{
    border-bottom: 0 !important;
    .btn-secondary{
      padding: 18px;
      background: $bg-color;
      border-radius: 16px;
      border: 0 !important;
      box-shadow: 0 0 0 !important;
    }
    .counter{
      position: relative;
      display: inline-block;
    }
    .counter::after{
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 2px;
      height: 30px;
      background: $light-300;
    }
  }
  .arrow{
    background: $dark-300;
    padding: 10px;
    border-radius: 10px;
    svg{
      transition: .3s;
    }
  }
}
</style>
