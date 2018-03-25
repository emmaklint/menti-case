<template>
<div>
  <div>
  <button class="grow button border-radius no-border sky small white poppins shadow bold pd-button" type="submit" name="submit" :value="msg.msg">{{msg.msg}}</button>
  </div>
</div>
</template>

<script>
export default {
  name: 'Intro',
  props: ['msg']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.button {
  min-width: 250px;
  align-self: flex-start;
}
</style>
