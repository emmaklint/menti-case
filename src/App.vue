<template>
  <div id="app">
    <Intro/>
    <div class="container row align-center content-center">
      <Feature/>
      <Feature/>
      <Feature/>
    </div>
    <div class="container column">
    </div>
  </div>
</template>

<script>
import Intro from './components/Intro'
import Feature from './components/Feature'
import Submit from './components/Submit'


export default {
  name: 'App',
  components: {
    Intro,
    Feature,
    Submit
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
  font-weight: 600;
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

.center { text-align: center }

.margin-auto { margin: auto;}
.m-0 { padding: 0 }

.pd-0 { padding: 0 }
.pd-10 { padding-left: 10%; padding-right: 10%}
.pd-20 { padding-left: 20%; padding-right: 20%}


.border-radius { border-radius: 10px;}

.container { display: flex; }
.row { flex-direction: row }
.column { flex-direction: column }

.content-center { justify-content: center }
.align-center { align-items: center}



</style>

/* Rectangle 2 Copy 4: */
background: #009FB8;
box-shadow: 0 2px 4px 0 rgba(0,0,0,0.50);
border-radius: 10px;
/* Get your free trial: */
font-family: Poppins-SemiBold;
font-size: 20px;
color: #FFFFFF;
letter-spacing: 0;
text-align: center;
line-height: 60px;
