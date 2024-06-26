<template>
  <main class="w-100 px-5">
    <course-head></course-head>
    <course-description></course-description>
    <course-items-list></course-items-list>
    <course-creator></course-creator>
    <course-comments></course-comments>
    <newsletter></newsletter>
  </main>
</template>

<script>
import CourseComments from '~/components/views/courseComments.vue';
import CourseCreator from '~/components/views/courseCreator.vue';
import CourseDescription from '~/components/views/courseDescription.vue';
import courseHead from '~/components/views/courseHead.vue';
import CourseItemsList from '~/components/views/courseItemsList.vue';
import Newsletter from '~/components/views/newsletter.vue';
export default{
  components:{
    courseHead,
    CourseDescription,
    CourseItemsList,
    CourseCreator,
    CourseComments,
    Newsletter,
  }
}
</script>

<style lang="scss" scoped>

</style>
