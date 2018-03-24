<template>
  <div class="textbox white">
    <h2 class="bold left"> {{item.title}}</h2>
    <p class="text left small"> {{item.message}}</p>
  </div>
</template>

<script>
export default {
  name: 'Feature',
  data () {
    return {
      title: "Security",
      message: "Ensure that all data stays within the organization"
    }
  },
  props: ['item']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.textbox { max-width: 500px;}
</style>
