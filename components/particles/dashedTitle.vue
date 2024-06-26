<template>
  <h2 :class="`d-flex align-items-center ${classList}`">
    <span v-if="dashedSide === 'both'" class="right d-block w-100 ml-2">
      <span class="cover"></span>
    </span>
    <slot></slot>
    <span class="left d-block w-100 mr-2">
      <span class="cover"></span>
    </span>
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
