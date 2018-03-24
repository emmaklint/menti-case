<template>
  <div class="textbox white container column m-0 p-5">
    <h2 class="bold left"> {{item.title}}</h2>
    <p class="text left small m-0"> {{item.message}}</p>
    <Submit class="space-button" :msg="{msg: item.msg}"/>
  </div>
</template>

<script>
import Submit from './Submit'

export default {
  name: 'Feature',
  components: {
    Submit
  },
  props: ['item']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h2 {font-size: 180%; margin-bottom: 0}
</style>
