<template>
  <h2 :class="`d-flex align-items-center ${classList}`">
    <span v-if="dashedSide === 'both'" class="right d-block w-100 ml-2">
      <span class="cover"></span>
    </span>
    <slot></slot>
    <span class="left d-block w-100 mr-2">
      <span class="cover"></span>
    </span>
    <p class="p-size-big font-reg mt-2">
      امتیاز کل دوره:
      <span class="pr-1">
        ۴.۸
        <svg width="18" height="18" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M7.9974 0.833328C8.69691 0.833328 9.24792 1.36168 9.59969 2.0746L10.7744 4.44344C10.81 4.51675 10.8944 4.61998 11.0214 4.71442C11.1482 4.80876 11.2724 4.8608 11.3541 4.87453L13.4805 5.23075C14.2486 5.35982 14.8924 5.73632 15.1014 6.39193C15.3102 7.04699 15.0042 7.72773 14.4519 8.28109L14.4514 8.28163L12.7994 9.94723C12.7339 10.0132 12.6606 10.1376 12.6146 10.2996C12.5689 10.4605 12.5649 10.6071 12.5856 10.7018L12.5859 10.7031L13.0585 12.7636C13.2545 13.6212 13.1896 14.4715 12.5847 14.9161C11.9778 15.3622 11.1485 15.1645 10.395 14.7157L8.4017 13.526C8.318 13.476 8.17424 13.4355 8.00073 13.4355C7.82849 13.4355 7.68171 13.4755 7.59256 13.5273L7.5913 13.5281L5.60192 14.7155C4.84937 15.1658 4.02103 15.36 3.41407 14.9135C2.80966 14.4688 2.74143 13.62 2.93807 12.7631L3.4106 10.7031L3.41089 10.7018C3.43161 10.6071 3.42755 10.4605 3.38187 10.2996C3.33587 10.1376 3.26252 10.0132 3.19705 9.94723L1.5439 8.28042C0.995098 7.72708 0.690138 7.04693 0.897298 6.39283C1.10506 5.73682 1.74762 5.35986 2.51622 5.2307L4.64088 4.87479L4.64156 4.87467C4.71945 4.86116 4.8418 4.8097 4.96832 4.71512C5.09507 4.62036 5.17973 4.5169 5.21541 4.44344L5.21721 4.43977L6.39041 2.07398L6.39088 2.07304C6.74597 1.36071 7.29869 0.833328 7.9974 0.833328Z" fill="#DE8208"/>
        </svg>
      </span>
    </p>
  </h2>
</template>

<script>
  export default {
    props:{
      dashedSide:{
        default: 'left'
      },
      classList:{
        default: ''
      }
    }
  }
</script>

<style lang="scss" scoped>
h2{
  white-space: nowrap;
  >span{
    border-bottom: 2px dashed $light-700;
    position: relative;
    .cover{
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      height: 2px;
      background: linear-gradient(to left , transparent , $secondary-color);
    }
  }
  .right{
    .cover{
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      height: 2px;
      background: linear-gradient(to right , transparent , $secondary-color);
    }
  }
}

</style>
