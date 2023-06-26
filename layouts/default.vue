< >
  <div class="page-wrapper">
    <nuxt />
  </div>
</ >


<script>

  export default {
    components: {
    },
    head(){
      return {
        title: "Apiton - Vue Nuxt App Landing Page  "
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
