<template>
  <div class="feature white-background margin-auto pd-box border-radius box-size shadow">
    <img class="icon" src="../assets/security.png"/>
    <h3 class="bold"> {{item.title}}</h3>
    <p class="text center small"> {{item.message}}</p>
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
.icon { width: 100px}
</style>
