<template>
   <div>
       <h5 id="header" class="text-center text-uppercase my-4" :class="{'dark' : dark , 'light': light}">{{ title }}</h5>
   </div>
</template>
<style lang="scss" scoped>
    .dark {
        color: $dark
    }
    .light {
        color: $light;
    }
</style>
<script>
export default {
  props: {
    title: {
      type: String,
      default: 'sem título'
    },
    dark: {
      type: Boolean,
      default: false,
      useDefaultForNull: true
    },
    light: {
      type: Boolean,
      default: false,
      useDefaultForNull: true
    }
  }
}
</script>
