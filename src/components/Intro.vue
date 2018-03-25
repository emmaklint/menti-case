<template>
  <div class="intro full container column content-center align-center">
      <div>
        <img class="logo" src="../assets/menti.png">
      </div>
      <h1 class="center bold white pd-25">Get your whole team presenting like superstars</h1>
      <p class="text center small white pd-25">Mentimeter is an easy­-to-­use tool that makes facilitators and presenters look like stars. No installations or downloads required ­- perfect for teams and organizations. For organizations of 2 or more users, Mentimeter for Teams gives you central control of licenses and knowledge shared within your organization.</p>
      <form class="container row form pd-10 m-2">
        <input class="flex-grow-2 input pd-button shadow border-radius no-border small poppins flex-grow space-horisontal" type="email" name="email" placeholder="Enter your email here">
        <Submit class="flex-grow-1 space-horisontal" :msg="{msg: 'Get your free trial'}"/>
      </form>
  </div>
</template>

<script>
import Submit from './Submit'

export default {
  name: 'HelloWorld',
  components: {
    Submit
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.full { min-height: 100vh}
h1 { font-size:60px; line-height: 120%}

.input { min-width: 400px; }

</style>
