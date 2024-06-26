<template>
  <header class="w-100 sticky-top pt-4">
    <div class="head-template p-1">
      <b-navbar toggleable="lg" class="">
        <b-navbar-brand href="#">
          <img width="150px" class="img-to-white" src="/logo.png" alt="">
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>

          <b-navbar-nav class="d-flex gap-3">
            <b-nav-item class="p-size-big font-reg" href="#">صفحه اصلی</b-nav-item>
            <b-nav-item class="p-size-big font-reg" href="#">لیست دوره‌ها</b-nav-item>
            <b-nav-item class="p-size-big font-reg" href="#">تماس با ما</b-nav-item>
            <b-nav-item class="p-size-big font-reg" href="#">درباره ما</b-nav-item>
          </b-navbar-nav>

          <div class="mr-auto">
            <btn classList="font-med p-size-big" size="lg" color="secondary" rounded="xl">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M18 19C18 16.7909 15.3137 15 12 15C8.68629 15 6 16.7909 6 19M12 12C9.79086 12 8 10.2091 8 8C8 5.79086 9.79086 4 12 4C14.2091 4 16 5.79086 16 8C16 10.2091 14.2091 12 12 12Z" stroke="white" stroke-width="1.3" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              حساب کاربری
            </btn>
          </div>

        </b-collapse>
      </b-navbar>
    </div>
  </header>
</template>

<script>
import btn from '../particles/btn.vue'
export default {
  components: { btn },

}
</script>

<style lang="scss" scoped>
header{
  z-index: 1111111 !important;
  .head-template{
    background: $bg-color;
    border-radius: 48px;
  }
}
</style>
