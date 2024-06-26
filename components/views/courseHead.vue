<template>
  <div class="course-head py-4 px-5 mt-5 d-flex gap-4 justify-content-between align-items-center">
    <div class="py-3">
      <h1 class="font-bold h1-size">
        الگوهای طراحی حرفه ای - #C
      </h1>
      <a href="" class="d-flex gap-3 mt-4 pt-3 align-items-center">
        <img loading="lazy" width="48px" src="/img/icons/user-photo.png" alt="user" />
        <span class="d-flex flex-column gap-1 opacity-900">
          احمدرضا شاه ‌محمدی
          <span class="opacity-700">
            Senior Backend developer
          </span>
        </span>
      </a>
    </div>
    <div class="rate-box p-4 d-flex opacity-900">
      <div class="d-flex flex-column justify-content-between px-2">
        <span class="d-flex top-box pb-4 mb-3 font-med gap-3 h5-size">
          <svg width="30" height="30" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M5.83333 11.6666V18.6796C5.83333 19.0984 5.83333 19.3078 5.8971 19.4926C5.95348 19.6561 6.04551 19.805 6.16651 19.9285C6.30334 20.0683 6.49063 20.1619 6.8652 20.3492L13.1652 23.4992C13.4713 23.6522 13.6243 23.7288 13.7849 23.7589C13.927 23.7855 14.0729 23.7855 14.2151 23.7589C14.3757 23.7288 14.5287 23.6522 14.8348 23.4992L21.1348 20.3492C21.5094 20.1619 21.6967 20.0683 21.8335 19.9285C21.9545 19.805 22.0465 19.6561 22.1029 19.4926C22.1667 19.3078 22.1667 19.0984 22.1667 18.6796V11.6666M2.33333 9.91658L13.5826 4.29195C13.7356 4.21542 13.8122 4.17716 13.8924 4.1621C13.9635 4.14877 14.0365 4.14877 14.1076 4.1621C14.1878 4.17716 14.2644 4.21542 14.4174 4.29195L25.6667 9.91658L14.4174 15.5412C14.2644 15.6177 14.1878 15.656 14.1076 15.6711C14.0365 15.6844 13.9635 15.6844 13.8924 15.6711C13.8122 15.656 13.7356 15.6177 13.5826 15.5412L2.33333 9.91658Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
          دوره آنلاین
        </span>
        <span class="d-flex font-med pt-1 gap-3 h5-size">
          <svg width="28" height="28" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M14 6.99992V13.9999L18.6667 16.3333M25.6667 13.9999C25.6667 20.4432 20.4433 25.6666 14 25.6666C7.55668 25.6666 2.33333 20.4432 2.33333 13.9999C2.33333 7.5566 7.55668 2.33325 14 2.33325C20.4433 2.33325 25.6667 7.5566 25.6667 13.9999Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
          ۲۷ ساعت
        </span>
      </div>
      <div class="d-flex justify-content-center pr-4 mr-3 pl-2 left-box flex-column align-items-center font-med gap-3 h5-size">
        <svg width="31" height="31" viewBox="0 0 29 29" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M16.5156 4.51813L18.5687 8.65827C18.8486 9.2346 19.5952 9.7874 20.2252 9.89326L23.9464 10.5166C26.3262 10.9165 26.8861 12.6573 25.1713 14.3745L22.2783 17.2914C21.7883 17.7854 21.52 18.7381 21.6717 19.4203L22.4999 23.0312C23.1532 25.8893 21.6483 26.9949 19.1403 25.5011L15.6523 23.4193C15.0224 23.0429 13.9842 23.0429 13.3426 23.4193L9.85464 25.5011C7.35825 26.9949 5.84175 25.8775 6.49501 23.0312L7.32325 19.4203C7.4749 18.7381 7.2066 17.7854 6.71665 17.2914L3.82364 14.3745C2.12049 12.6573 2.66877 10.9165 5.04851 10.5166L8.76976 9.89326C9.38803 9.7874 10.1346 9.2346 10.4146 8.65827L12.4677 4.51813C13.5876 2.27163 15.4074 2.27163 16.5156 4.51813Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
        ۴.۸
      </div>
    </div>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.course-head{
  background: $bg-color;
  border-radius: 25px;
  .rate-box{
    border: 2px solid $light-200;
    border-radius: 15px;
  }
  .left-box{
    border-right: 2px solid $light-200;
  }
  .top-box{
    border-bottom: 2px solid $light-200;
  }
}
</style>
