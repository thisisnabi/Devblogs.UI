<template>
  <a :href="url" v-if="base === 'a'" :class="`btn ${color} radius-${size} ${rounded} ${classList}`">
    <slot></slot>
  </a>
  <nuxt-link v-else-if="base === 'nuxt'" :class="`btn ${color} ${size} radius-${rounded} ${classList}`" :to="url">
    <slot></slot>
  </nuxt-link>
  <button :class="`btn ${color} ${size} radius-${rounded} ${classList}`" v-else>
    <slot></slot>
  </button>
</template>

<script>
  export default {
    props:{
      base:{
        default: 'btn',
      },
      color:{
        default: 'primary'
      },
      size: {
        default: 'md',
      },
      url: {
        default: '/'
      },
      classList:{
        default: ''
      },
      rounded:{
        default: 'md'
      }
    }
  }
</script>

<style lang="scss" scoped>
.btn{
  cursor: pointer;
}
.primary{
  background: $primary-color;
  color: $text-color;
  border: 2px solid $primary-color;
}
.light{
  background: $light-color;
  color: $dark-color;
  border: 2px solid $light-color;
}
.secondary{
  background: transparent;
  color: $text-color;
  border-radius: 9px;
  border: 2px solid $light-300;
}
.md{
  padding: 10px 22px;
}
.lg{
  padding: 13px 26px;
}
.radius-md{
  border-radius: 9px;
}
.radius-xl{
  border-radius: 31px;
}
</style>
