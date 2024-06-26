<template>
  <div class="backdrop">
    <div :class="numbers.includes(i) ? 'active' : ''" v-for="i in 55" :key="i"></div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        numbers: []
      }
    },
    mounted(){
      this.generateRandomNumbers()
    },
    methods:{
      generateRandomNumbers() {
        let numbers = [];
        while (numbers.length < 8) {
          let randomNumber = Math.floor(Math.random() * 55) + 1;
          if (!numbers.includes(randomNumber)) {
            numbers.push(randomNumber);
          }
        }
        let minDistance = 5;
        for (let i = 0; i < numbers.length - minDistance; i++) {
          let distance = numbers[i + minDistance] - numbers[i];
          if (distance < minDistance) {
            let diff = minDistance - distance;
            numbers[i + minDistance] += diff;
          }
        }
        this.numbers = numbers;
        this.numbers.push(1)
        this.numbers.push(22)
        this.numbers.push(23)
        this.numbers.push(50)
      }
    }
  }
</script>

<style lang="scss" scoped>
.backdrop{
  position: absolute;
  z-index: -3;
  top: -2px;
  left: -2px;
  right: -2px;
  display: grid;
  grid-template-columns: repeat(11 , 1fr);
  div{
    position: relative;
    height: 125px;
    border: 1px solid $light-100;
    border-top-width: 2px;
    border-bottom: 0;
    opacity: .6;
    z-index: -3;
  }
  .active{
    background: $bg-color;
  }
}
.backdrop::after{
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: -1;
  background: linear-gradient(to bottom , transparent , transparent,$secondary-color);
}
</style>
