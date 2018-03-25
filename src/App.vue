<template>
  <div id="app">
    <Intro/>
    <div class="container column content-space">
      <div class="container row wrap align-center content-center margin-auto space">
        <Feature :item="{title: 'Easy administration', message: '­ Central administration and billing with one invoice.', icon: 'paper'}"/>
        <Feature :item="{title: 'Increase collaboration', message: 'Share your presentations and create knowledge hub', icon: 'collaboration'}"/>
        <Feature :item="{title: 'Secure', message: 'Ensure that all data stays within the organization', icon: 'lock'}"/>
      </div>
      <div class="container column">
        <div class="container row wrap content-space space">
          <Textbox class="flex-half" :item="{title: 'Mentimeter for business features', message: '­Mentimeter is an easy­to­use presentation software used by more than 8 million people. With Mentimeter you can create fun and interactive presentations. We help you make your events, presentations, lectures, and workshops innovative and memorable. Perfect for businesses that want to grow and take care of their employees.', msg: 'Learn more about features'}"/>
          <div class="flex-half">
            <img src="./assets/logo.png"/>
          </div>
        </div>
        <div class="container row wrap-reverse content-space space">
          <div class="flex-half">
            <img src="./assets/MichaelScott.png"/>
          </div>
          <Textbox class="flex-half" :item="{title: 'Customers grow with Mentimeter', message: 'Praxent helps customers grow through custom software and have used Mentimeter to help them grow their business. Director of Operations, Chris Walker gave us an insight into how Mentimeter has helped Praxent, his thoughts have been reflected in this blog post.', msg: 'Read the full story'}"/>
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
  color: #2c3e50;
  width: 100vw;
}

.text { font-family: 'Open Sans', sans-serif }
.small {font-size: 1.2em}
.bold { font-weight: 600}
.white {color: white}
.white-background { background-color: white}
.sky {background-color: #009fb8}
.poppins {font-family: 'Poppins'; font-weight: 600}

.left { text-align: left }
.center { text-align: center }

.margin-auto { margin: auto;}
.m-0 { margin: 0 }
.m-2 { margin: 2% 0}
.m-10 { margin: 10% }
.space {margin: 5% 0}
.space-horisontal {margin: 0 2%}

.pd-0 { padding: 0 }
.pd-5 { padding-left: 5%; padding-right: 5%}
.pd-10 { padding-left: 10%; padding-right: 10%}
.pd-20 { padding-left: 20%; padding-right: 20%}
.pd-25 { padding-left: 25%; padding-right: 25%}
.pd-30 { padding-left: 30%; padding-right: 30%}

.auto-width {  object-fit: cover;}

.no-border { border: 0 }

.pd-button { padding: 10px 25px}
.space-button {margin-top: 3%; margin-bottom: 3%}

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

.flex-half {max-width: 500px;}
.flex-grow-1 { flex-grow: 1 }
.flex-grow-2 { flex-grow: 2 }
.wrap {flex-wrap: wrap}
.wrap-reverse {flex-wrap: wrap-reverse}


.logo {width:400px;}

.grow { transition: all .2s ease-in-out; }
.grow:hover { transform: scale(1.05); }
</style>
