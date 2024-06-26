<template>
  <div class="course-card p-2">
    <img class="w-100" src="/img/design/programing.png" alt="">
    <h2 class="font-med h4-size mt-4">
      <a href="">
        برنامه نویسی سی شارپ
      </a>
    </h2>
    <p class="h6-size opacity-800 pt-1">
      دوره بهینه سازی در React یک دوره ویژه برای React کارهاست تا کدبهتری با سرعت بالاتری در React بنویسند
    </p>
    <a href="/" class="link d-flex justify-content-between align-items-center w-100 mt-4 mb-1">
      <span>
        <img width="33px" class="ml-2" loading="lazy" src="/img/icons/user-photo.png" alt="user-photo">
        امیررضا باقری
      </span>
      <svg width="27" height="27" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M11.6666 13.3333L8.33325 9.99996L11.6666 6.66663" stroke="white" stroke-width="1.3" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </a>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.course-card{
  background: $bg-color;
  border-radius: 12px;
  .link{
    background: $dark-200;
    border-radius: 12px;
    padding: 12px;
    padding-left: 4px;
  }
  img{
    border-radius: 12px;
  }
}
</style>
