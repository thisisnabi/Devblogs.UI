<template>
  <footer class="row p-4 mb-5">
    <div class="col-3 menu">
      <h4 class="font-med pb-3 d-inline-block pl-5">
        دسترسی سریع
      </h4>
      <ul class="mt-3 d-flex flex-column gap-2 p-size-big pr-4">
        <li v-for="i in 3" :key="i" :class="i === 1 ? 'active': ''">
          <a href="" class="pt-1 d-inline-block">
            تماس باما
          </a>
        </li>
      </ul>
    </div>
    <div class="col-3 menu">
      <h4 class="font-med pb-3 d-inline-block pl-5">
        دوره های محبوب
      </h4>
      <ul class="mt-3 d-flex flex-column gap-2 p-size-big pr-4">
        <li v-for="i in 3" :key="i" :class="i === 2 ? 'active': ''">
          <a href="" class="pt-1 d-inline-block">
            آموزش دات نت
          </a>
        </li>
      </ul>
    </div>
    <div class="col-6 info">
      <div class="d-flex align-items-end gap-5 mb-4 pb-1">
        <div class="">
          <h4 class="font-med pb-3 ml-4">
            يادگیری از همین جا شروع میشه
          </h4>
          <p class="p-size-big opacity-800 mb-0">
            لورم ایپسوم متن ساختگی   لورم ایپسوم متن ساختگی  لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه
          </p>
        </div>
        <div class="bg-dark enamad d-flex align-items-center justify-content-center">
          اینماد
        </div>
      </div>
      <div class="social-media mt-2 p-size-big p-3 d-flex justify-content-between align-items-center">
        شبکه‌های اجتماعی
        <div class="d-flex gap-4 px-1">
          <a v-for="i in 3" :key="i" href="/">
            <img width="25px" src="/img/icons/linkedin-02.svg" alt="">
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
footer{
  background: $bg-color;
  margin-top: 100px !important;
  border-radius: 16px;
  .info{
    p{
      line-height: $h2-size;
    }
    .enamad{
      width: 230px;
      height: 95px;
      border-radius: 10px;
    }
    .social-media{
      background: $dark-500;
      border-radius: 13px;
    }
  }
  .menu{
    h4{
      border-bottom: 2px solid $light-200;
    }
    ul{
      li.active{
        color: $primary-color;
        a{
          color: $primary-color !important;
        }
      }
    }
  }
}
</style>
