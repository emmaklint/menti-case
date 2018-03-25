<template>
  <div class="container column align-center grow feature white-background margin-auto pd-box border-radius box-size shadow">
    <img class="icon center" :src= "src"/>
    <h3 class="bold center"> {{item.title}}</h3>
    <p class="text center small m-0"> {{item.message}}</p>
  </div>
</template>

<script>
export default {
  name: 'Feature',
  props: ['item'],
  computed: {
    src () {
      return require('../assets/' + this.item.icon + '.png')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.icon { width: 200px}
</style>
