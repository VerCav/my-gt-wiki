<template>
    <div>
      <AppBanner />
      <nuxt />
    </div>
  </template>
  
  <script>
  import AppBanner from '~/components/AppBanner.vue'
  
  export default {
    components: {
      AppBanner,
    }
  }
  </script>
  