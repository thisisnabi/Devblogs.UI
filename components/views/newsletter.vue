<template>
  <div class="newsletter p-5 mt-5 d-flex flex-column align-items-center justify-content-center">
    <h3 class="font-demi h2-size mb-3 pb-1">
      عضویت در خبرنامه
    </h3>
    <p class="h5-size pb-4">
      با عضویت در خبرنامه می توانید از جدیدترین تخفیف‌ها، دوره‌ها، رویدادها و... با اطلاع شوید.
    </p>
    <form class="">
      <input placeholder="ایمیل شما" class="input-form" type="email" />
      <btn classList="h4-size font-med mr-2 px-4">
        <svg width="30" height="29" viewBox="0 0 33 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M20.5 25.3334C20.5 22.3879 16.9183 20 12.5 20C8.08172 20 4.5 22.3879 4.5 25.3334M25.8333 21.3334V17.3334M25.8333 17.3334V13.3334M25.8333 17.3334H21.8333M25.8333 17.3334H29.8333M12.5 16C9.55448 16 7.16667 13.6122 7.16667 10.6667C7.16667 7.72119 9.55448 5.33337 12.5 5.33337C15.4455 5.33337 17.8333 7.72119 17.8333 10.6667C17.8333 13.6122 15.4455 16 12.5 16Z" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
        عضویت
      </btn>
    </form>
  </div>
</template>

<script>
import btn from '../particles/btn.vue'
export default {
  components: { btn },

}
</script>

<style lang="scss" scoped>
.newsletter{
  border-radius: 24px;
  border: 3px dashed $light-100;
  input{
    width: 450px;
    min-width: 250px !important;
  }
}
</style>
