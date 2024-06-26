<template>
  <section class="container-fluid h-100 w-100">
    <backdrop-filter></backdrop-filter>
    <header-default></header-default>
    <nuxt />
    <footer-default></footer-default>
  </section>
</template>

<script>
import BackdropFilter from '~/components/particles/backdropFilter.vue'
import FooterDefault from '~/components/views/footerDefault.vue'
import headerDefault from '~/components/views/headerDefault.vue'
export default {
  components: { headerDefault, FooterDefault, BackdropFilter },
  name: 'defaultLayout',
}
</script>

<style lang="scss" scoped>
.container-fluid{
  padding: 0 100px !important;
}
</style>
