<template>
  <main class="w-100 px-5 py-5">
    <search></search>
    <div class="row mt-5">
      <div v-for="i in 12" :key="i" class="col-3 px-2">
        <course-card class="mb-4 mx-1"></course-card>
      </div>
    </div>
  </main>
</template>

<script>
import CourseCard from '~/components/particles/courseCard.vue'
import search from '~/components/particles/search.vue'
export default {
  components: { search, CourseCard },
}
</script>

<style lang="scss" scoped>

</style>
