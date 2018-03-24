<template>
  <div id="app">
    <Intro/>
    <div class="container column content-space">
      <div class="container row align-center content-center margin-auto space">
        <Feature :item="{title: 'Easy administration', message: '­ Central administration and billing with one invoice.'}"/>
        <Feature :item="{title: 'Increase collaboration', message: 'Share your presentations and create knowledge hub'}"/>
        <Feature :item="{title: 'Secure', message: 'Ensure that all data stays within the organization'}"/>
      </div>
      <div class="container column">
        <div class="container row content-space align-center space">
          <Textbox :item="{title: 'Mentimeter for business features', message: '­Mentimeter is an easy­to­use presentation software used by more than 8 million people. With Mentimeter you can create fun and interactive presentations. We help you make your events, presentations, lectures, and workshops innovative and memorable. Perfect for businesses that want to grow and take care of their employees.'}"/>
          <img src="./assets/logo.png"/>
        </div>
        <div class="container row content-space align-center space">
          <img src="./assets/MichaelScott.png"/>
          <Textbox :item="{title: 'Customers grow with Mentimeter', message: 'Praxent helps customers grow through custom software and have used Mentimeter to help them grow their business. Director of Operations, Chris Walker gave us an insight into how Mentimeter has helped Praxent, his thoughts have been reflected in this blog post.'}"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Intro from './components/Intro'
import Feature from './components/Feature'
import Submit from './components/Submit'
import Textbox from './components/Textbox'

export default {
  name: 'App',
  components: {
    Intro,
    Feature,
    Submit,
    Textbox
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background: linear-gradient(to bottom right, #162F37, #315C68);
}

#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.text { font-family: 'Open Sans', sans-serif }
.small {font-size: 1.2em}
.bold { font-weight: 600}
.white {color: white}
.white-background { background-color: white}
.sky {background-color: #009fb8}

.left { text-align: left }
.center { text-align: center }

.margin-auto { margin: auto;}
.m-0 { padding: 0 }
.m-10 { margin: 10% }
.space {margin-top: 10%; margin-bottom: 10%}

.pd-0 { padding: 0 }
.pd-10 { padding-left: 10%; padding-right: 10%}
.pd-20 { padding-left: 20%; padding-right: 20%}
.pd-30 { padding-left: 30%; padding-right: 30%}


.pd-button { padding: 10px;}

.pd-box {padding: 2%}
.box-size {max-width: 300px; min-height: 200px;}
 
.border-radius { border-radius: 10px;}
.shadow {box-shadow: 0 2px 4px 0 #162F37; }


.container { display: flex; }
.row { flex-direction: row }
.column { flex-direction: column }

.content-center { justify-content: center }
.content-space { justify-content: space-around }
.align-center { align-items: center}

</style>