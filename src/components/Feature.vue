<template>
  <div class="container column align-center grow feature white-background margin-auto pd-box border-radius box-size shadow">
    <img class="icon center" src="../assets/security.png"/>
    <h3 class="bold center"> {{item.title}}</h3>
    <p class="text center small m-0"> {{item.message}}</p>
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
.icon { width: 80px}
</style>
