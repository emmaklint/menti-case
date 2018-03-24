<template>
<div>
  <div>
  <input class="grow border-radius no-border sky small white poppins shadow bold pd-button" type="submit" name="submit" :value="msg.msg">
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
  display: inline;
}

</style>
