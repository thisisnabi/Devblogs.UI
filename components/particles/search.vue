<template>
  <div class="py-4 my-2">
    <h1 class="font-demi pb-1 h2-size text-center">
      داستان برنامه‌نویس شدنت از اینجا شروع میشه!
    </h1>
    <p class="h5-size text-center pt-2 opacity-900">
      یادگیری برنامه‌نویسی آرزو نیست، فقط نیاز هست، تلاش و تمرین داشته باشید، بقیه‌اش با راکت
    </p>

    <form action="" class="d-flex align-items-center justify-content-center mt-5">
      <div>
        <input placeholder="چه چیزی دوست داری یاد بگیری؟" class="input-form" />
        <btn color="light" classList="font-med">
          <svg width="21" height="20" viewBox="0 0 19 18" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M16.25 15.75L13.6251 13.125M15.5 8.625C15.5 12.1458 12.6458 15 9.125 15C5.60418 15 2.75 12.1458 2.75 8.625C2.75 5.10418 5.60418 2.25 9.125 2.25C12.6458 2.25 15.5 5.10418 15.5 8.625Z" stroke="#0C111E" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
          جستجو
        </btn>
      </div>
    </form>

    <div class="d-flex justify-content-center mt-3 pb-3">
      <div class="popular-search">
        <span>System Design</span>
        <span>ASP</span>
        <span class="active">System Design</span>
        <span>ASP.NET Core</span>
      </div>
    </div>
  </div>
</template>

<script>
import btn from '../particles/btn.vue'
export default {
  components: { btn },

}
</script>

<style lang="scss" scoped>
.popular-search{
  background: $bg-color;
  border-radius: 100px;
  padding: 13px 12px !important;
  padding-top: 16px !important;
  span{
    padding: 6px 22px;
    padding-top: 8px;
    border-radius: 100px;
    cursor: pointer;
    font-weight: 600;
    color: $light-700;
  }.active{
    background: $dark-300;
  }
}
form{
  div{
    position: relative;
    input{
      width: 530px;
      border-radius: 100px;
      font-size: $p-size-big;
      padding: 16px ;
    }
    button{
      border-radius: 100px !important;
      position: absolute;
      left: 9px;
      top: 7.5px;
    }
  }
}
</style>
