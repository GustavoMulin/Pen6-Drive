<template>
  <div class="page-wrapper">
    <nuxt />
  </div>
</template>


<script>
import 'material-icons/iconfont/material-icons.css';

  export default {
    components: {
    },
    head(){
      return {
        title: "P6.App"
      }
    },
    mounted(){
      this.$nextTick(() => {
        this.$nuxt.$loading.start()
        setTimeout(() => this.$nuxt.$loading.finish(), 500)
      })
    }
  }
</script>

<style>
</style>
