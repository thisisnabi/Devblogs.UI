<template>
  <main class="w-100 px-5 py-5">
    <search></search>
    <coming-soon></coming-soon>
  </main>
</template>

<script>
import search from '~/components/particles/search.vue'
import ComingSoon from '~/components/views/comingSoon.vue'
export default {
  components: { search, ComingSoon },
}
</script>

<style lang="scss" scoped>

</style>
